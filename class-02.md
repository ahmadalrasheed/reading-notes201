# class-02

## text

***When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.now we will talk about some of those tags***

### Headings

![headings](https://www.tutorialrepublic.com/lib/images/html/html-headings.png)

* `<h1>` > is used for main headings, the most important topic

* `<h2>` is used for subheadings, less important than `<h1>`

* `<h3>` is used for subheadings, less important than `<h2>`

* `<h4>` is used for subheadings, less important than `<h3>`

* `<h5>` is used for subheadings, less important than `<h4>`

* `<h6>` is used for subheadings, the least important subheading `<h5>`


### paragraphs

***To create a paragraph, surround the words that make up the paragraph with an opening `<p>` tag and closing `</p>` tag.***

**By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.**


### Bold & Italic

#### Bold

***By enclosing words in the tags <b> and </b> we can make characters appear bold.***


#### Italic

***By enclosing words in the tags `<i>` and `</i>` we can make characters appear italic.***

### Line Breaks & Horizontal Rules

![breakline](https://raw.githubusercontent.com/lennyroyroy/basics-image/master/linebreak-horizontal.png)

* `<br />` : As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag `<br />`.

* `<hr />`: To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the `<hr />` tag.


### Strong & Emphasis


* `<strong>` : The use of the `<strong>` element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis.

* `<em>` : The `<em>` element indicates emphasis that subtly changes the meaning of a sentence. By default browsers will show the contents of an `<em>` element in italic.


## Introducing CSS

**In this section, we will look at how to make your web pages more attractive, controlling the design of them using CSS.**

![CSS](https://www.freetutorialsplus.com/css-tutorial/images/css-illustration.png)

***CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that the background of the page is cream, all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.***


***there is three ways for using CSS And combine it with HTML which are :***

* inline CSS : it by using CSS inside the HTML code.

`example: <h1 style="color:blue;text-align:center;">This is a heading</h1>`

* internal CSS: You can also include CSS rules within an HTML page by placing them inside a `<style>` element, which usually sits inside the `<head>` element of the page.here is an example down below in the picture:

![internalCSS](https://i.stack.imgur.com/K59EF.gif)

* external CSS: its by combining our HTML code with CSS external sheet by the following command in the `<head>`, here is the example below:


`<link href="CSSsheetname" type="text/css"`



**in the picture below we will see a picture which describes clearly all types of CSS, see the following picture:**

![externalCSS](https://www.bitdegree.org/learn/storage/media/images/8c4493d3-110c-4a95-8b70-7626ce2d2f4e.jpg)


## basic javascript instructions

***you will start learning to read and write JavaScript. You will also learn how to give a web browser instructions you want it to follow.*** 

![javascript](https://res.cloudinary.com/practicaldev/image/fetch/s--_pyWGSyD--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://thepracticaldev.s3.amazonaws.com/i/w9u60357jk4ozdho7urq.jpg)



### STATEMENTS 

A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement Statements should end with a semicolon. 

**examples:**

* `var today= new Date{);`

* `var hourNow = today.getHours{) ;`

* `var greeting; `

### COMMENTS

***You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.***

`example: // Declare x, give it the value of 5`

#### WHAT IS A VARIABLE? 

***A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.***

#### variables:how to declare them?

* its by using `var` then the name of the variable that you want

`example: var quantity;`

#### variables: how to assign them a value

* its by putting a value after the assignment operator `=`


`example: quantity=3;`











