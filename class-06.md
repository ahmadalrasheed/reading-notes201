## WHAT IS AN OBJECT?

***Objects group together a set of variables and functions to  create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.***

![objects](https://miro.medium.com/max/2722/1*iKJx57JU9sKdff-Os7upyA.png)

**This object represents a hotel. It has five properties and one method. The object is in curly braces. It is stored in a variable called hotel .***

> var hotel={
    name:'quay';
    rooms:40;
    booked:25;
    gym:true;
    roomtypes:['twin','double','suite']
    checkavailabality:function(){
        return this.rooms
    }
}




### Creating an Object: literal Notation

***literal notation is the easiest and most popular way to create objects.***

![terminology](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/How-to-Create-JavaScript-Objects-1200x675.jpg)


**here is the following example:**

> var hotel={
    name:'quay';
    rooms:40;
    booked:25;
    gym:true;
    roomtypes:['twin','double','suite']
    checkavailabality:function(){
        return this.rooms
    }
}



### Accessing an Object and dot Notation

you access the properties or methods of an object using dot notation. you also can access properties using square brackets.

**this is an example for accessing functions in objects:**


`var roomsfree=hotel.checkavailabality();`

## Document object Model

![objectsmodel](https://simplesnippets.tech/wp-content/uploads/2018/10/what-is-document-object-model-in-JS-featured-image.jpg)


***The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access  and update the contents of a web page while it is in the browser window.***

The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.It is implemented by all major browser makers, and covers two primary areas:

* MAKING A MODEL OF THE HTML PAGE

***When the browser loads a web page, it creates a model of the page in memory. The DOM specifies the way in which the browser should structure this model using a DOM tree. The DOM is called an object model because the model (the DOM tree) is made of objects. Each object represents a different part of the page loaded in the browser window.***



* ACCESSING AND CHANGING THE HTML PAGE 

***The DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser. You will hear people call the DOM an Application Programming Interface (API). User interfaces let humans interact with programs; APls let programs (and scripts) talk to each other. The DOM states what your script can "ask the browser about the current page, and how to tell the browser to update what is being shown to the user.***



**example of DOM in the following picture:**




![image](https://tariqaustralia.files.wordpress.com/2013/03/dom_tree.gif)
