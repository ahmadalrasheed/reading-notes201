# HTML Image.color.text
## Image :
***On the Internet, images are used for all kinds of reasons: to enhance websites, to illustrate stories, in ad displays, to present products or services, as stand-alone "a picture is worth a thousand words" meaning-rich tools, and sure, on social media.***

![image](https://acumbamail.com/blog/wp-content/uploads/2014/10/maquetacion-email-html.png)



### Image adding


***In order to put a simple image on a webpage, we use the *img* element. This is an empty element > meaning that it has no text content or closing tag that requires a minimum of one attribute to be useful — src (sometimes spoken as its full title, source. The src attribute contains a path pointing to the image you want to embed in the page, which can be a relative or absolute URL, in the same way as href attribute values in `*a*` element.***



#### Format my image: 
***Most normal image formats (JPEG, GIF, PNG, BMP, TIFF, SVG) will work in most situations most of the time.***



#### Edit my image :
***The traditional way to avoid this was to provide width and height attributes in the *img* markup so even when the browser has just the HTML, it is still able to allocate the appropriate amount of space.***
***Controlling Image Width: Before the advent of CSS, the display width of an image was controlled by the width attribute. This usage has been deprecated. In the absence of any CSS rules defining the display width of the image, it will still work in most browsers. However, this is specifically contrary to the HTML5 specification.***


***Responsive Image Widths:Generally speaking, you usually don't want to control the exact width of an image. Every visitor who comes to your website has a potentially different size screen. If you specify the width, it may be much too small for some users and much too big for others. Most of the time, the best option is to make sure that your image is inside of a responsive (percent-based) container and then let it fill the container.***


 **example of image in HTML:**




![LAB02](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2020/07/html-images-df.jpg)
-------




### HTML5: Figure and Figure Caption

**The HTML figure Figure With Optional Caption element represents self-contained content, potentially with an optional caption, which is specified using the *figcaption* element. The figure, its caption, and its contents are referenced as a single unit.**



## color
***Just starting your website or need a refresher? Our tutorials section has something for everyone, from basic HTML and CSS color guides to more advanced techniques in SCSS.***





***codes are ways of representing the colors we see everyday in a format that a computer can interpret and display. Commonly used in websites and other software applications, there are a variety of formats, including Hex color codes, RGB and HSL values, and HTML color names, amongst others.***
### HEX Color codes

***The most popular are Hex color codes; three byte hexadecimal numbers (meaning they consist of six digits), with each byte, or pair of characters in the Hex code, representing the intensity of red, green and blue in the color respectively.***
***Hex code byte values range from 00, which is the lowest intensity of a color, to FF which represents the highest intensity. The color white, for example, is made by mixing each of the three primary colors at their full intensity, resulting in the Hex color code of `#FFFFFF`.***


**example of HTML color**


![LAB02](http://www.urimagination.com/wp-content/uploads/2012/01/htmlColor1.png)
-------















## JPEG vs PNG vs GIF — which image format to use and when?
***Theres alot of image formats avaiable each one has a specific use case.we would only be looking and see three most common type used in website and mobile app,jpeg,png and gif.***


* jpeg : stands for "Joint Photographic Experts Group". It's a standard image format for containing lossy and compressed image data. Despite the huge reduction in file size JPEG images maintain reasonable image quality.
* png : stands for Portable Network Graphics and is another raster image type. The main difference between a PNG and a JPG is that a PNG file can have a transparent background and is generally larger and of higher quality. PNGs are great for interactive documents such as web pages but are not suitable for print.
* gif: The Graphics Interchange Format s a bitmap image format that was developed by a team at the online services provider CompuServe led by American computer .
![LAB5](https://s3.amazonaws.com/ckl-website-static/wp-content/uploads/2017/06/image-formats-cover-1280x680.png)

### Transparency
![htmlcss](https://www.pngitem.com/pimgs/m/23-237369_html5-and-css3-transparent-background-html-logo-hd.png)
***transparency indicates something that is completely invisible.we can use it to make logo and icons transparency to placed on background.***



* jpeg: images don't support transparency .
* png : it support transparency in two way,1- nserting an alpha channel that allows partial transparency or by declaring a single colour as transparen. 2 -Partial transparency makes the edges blend smoothly into the background. 
* gif: support transparency by declaring a single colour in the colour palette as transparent.
* color:
* jpeg :support around 16 million colours. This is what makes them suitable for storing images of natural scenes.
* png : NG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. Use PNG8 for simple shapes with fewer colours and PNG24 for high quality, complex logos and shapes with rounded corners on a transparent background.
* gif : are limited to 256 colours.

* Animation :You can upload multiple PNG or JPG images to our animated PNG maker, choose the order, frame duration and transition effect (if you want to), and it will assemble animated PNG from these images. With this method you can use the full potential of animated PNG and create images with much broader color palette than GIFs



 



## Text


![text](https://cdn.educba.com/academy/wp-content/uploads/2020/01/HTML-Justify-Text.jpg)


***The formatting of your text can have a significant effect on how readable your pages are. As we look through these properties I will also give you some design tips on how to display your type.***


### Typeface Terminology

![](data:image/png;base64,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)

### Serif

> Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.



### Sans-Serif

> Sans-serif fonts have straight
ends to letters, and therefore
have a much cleaner design.


### Monospace

> Every letter in a monospace (or
fixed-width) font is the same
width. (Non-monospace fonts
have different widths.)



