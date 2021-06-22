# class-04
## links

***Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.***


### Writing Links

![links](https://www.copahost.com/blog/wp-content/uploads/2019/07/html-link.jpg)

***Links are created using the `<a>` element. Users can click on anything between the opening `<a>` tag and the closing `</a>` tag. You specify which page you want to link to using the href attribute.***


**here is an example of the links code:**


`<a href="http://www.imdb.com">IMDB</a>`


### Opening Links in a New Window

#### target


**If you want a link to open in a new window, you can use the target attribute on the opening <a> tag. The value of this attribute should be _blank.**


**here is an example below:**


`<a href="http://www.imdb.com" target="_blank">`


## Layout


![layout](https://slideplayer.com/14545330/90/images/slide_1.jpg)

***r we are going to look at how to control where each element sits on a page and how to create attractive page layouts.***

### Key Concepts in Positioning Elements

#### Building Blocks


***CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box. Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors.***



#### Block-level elements

***start on a new line Examples include: `<h1> <p> <ul> <li>`***



#### Inline elements


***flow in between surrounding text Examples include: `<img>` `<b>` `<i>`***


### Controlling the Position of Elements


![positioning](https://i2.wp.com/css-tricks.com/wp-content/uploads/2020/07/Screen-Shot-2020-07-24-at-11.46.02-AM.png?resize=1024%2C663&ssl=1)

***CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property***



#### Normal flow

***Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior(unless you tell the browser to do something else).***




#### Relative Positioning

***This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.***







#### Absolute positioning



***This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.***




### Functions,methods & Objects


![functions](https://res.cloudinary.com/academind-gmbh/image/upload/f_auto,q_auto/c_fit,dpr_3.0,g_center,w_500/v1/academind.com/content/tutorials/javascript-functions-are-objects/functions-are-objects)


#### what is a function? 

***Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).***


***A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).The parentheses may include parameter names separated by commas: (parameter1, parameter2, ...) The code to be executed, by the function, is placed inside curly brackets: {}***



>function name(parameter1, parameter2, parameter3) {
>  // code to be executed
>}


#### calling a function

**first you must have declared function, after that you can call it by the following command:**



`name();`





