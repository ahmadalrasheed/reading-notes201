## LOCAL STORAGE FOR WEB APPLICATIONS

![img](https://love2dev.com/img/dm_tapeuqaeiw77-1200x630.jpg)

> ***persistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.***

> ***Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:***


* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over

* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)

* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful


**What we really want is**:


* a lot of storage space 


* on the client


* that persists beyond a page refresh


* and isn’t transmitted to the server


### INTRODUCING HTML5 STORAGE

![localstorage](https://media-exp3.licdn.com/dms/image/C4E12AQGMEQ2wCp6zaQ/article-cover_image-shrink_600_2000/0/1520059473378?e=1628121600&v=beta&t=IHd0nmS4LZsUlzhYxHfJw2mdY04S6MqzzVcjHFIfJIU)


***What I will refer to as “HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” The naming situation is made even more complicated by some related, similarly-named, emerging standards that I’ll discuss later in this chapter.***

***So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.***


### USING HTML5 STORAGE

***HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.***

> interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};


***Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception.***

***Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets. For example, this snippet of code:***

> var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);


### TRACKING CHANGES TO THE HTML5 STORAGE AREA

![changesHTML](https://images.slideplayer.com/13/3826154/slides/slide_18.jpg)

***If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.***

***The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports. (If you’ve done this before with other events, you can skip to the end of this section. Trapping the storage event works the same as every other event you’ve ever trapped. If you prefer to use jQuery or some other JavaScript library to register your event handlers, you can do that with the storage event, too.)***

> if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};

The handle_storage callback function will be called with a StorageEvent object, except in Internet Explorer where the event object is stored in window.event.
> function handle_storage(e) {
  if (!e) { e = window.event; }
}
