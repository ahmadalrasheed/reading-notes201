# class-03

## lists

![lists](http://ways2web.weebly.com/uploads/5/4/4/8/54485903/8033093_orig.png)

***There are lots of occasions when we need to use lists. HTML provides us with three different types:***

* Ordered lists: are lists where each item in the list is numbered.

* Unordered lists: are lists that begin with a bullet point

* Definition lists are made up of a set of terms along with the definitions for each of those terms.


### Ordered Lists

* The ordered list is created with the `<ol>` element

* Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag. (The li stands for list item.) Browsers indent lists by default


### Unordered Lists

* The unordered list is created with the `<ul>` element.

* Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag. (The li stands for list item.) Browsers indent lists by default.

### Definition Lists

* The definition list is created with the <dl> element and usually consists of a series of terms and their definitions. Inside the <dl> element you will usually see pairs of <dt> and <dd> elements.

* This is used to contain the term being defined (the definition term).

* This is used to contain the definition.




## Boxes

### Box dimensions


* By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties.


* The most popular ways to specify the size of a box are to use `pixels`, `percentages`, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size.

### Border, Margin & Padding

![border,margin](https://devopedia.org/images/article/289/5708.1602657423.png)

1. Border: Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.



2. Margin: Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.



3. Padding: Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.



**The padding and margin properties are very helpful in adding space between various items on the page.**


### Inline/Block Display



![inlineblock](https://www.differencebetween.com/wp-content/uploads/2018/02/Difference-Between-Block-and-Inline-Elements-fig-1.png)


***The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page.The values this property can take are:***

* inline: This causes a block-level element to act like an inline element.

* Block: This causes an inline element to act like a block-level element.

* inline-block: This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.




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



### CREATING AN ARRAY

***You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array***

![array](https://jarednielsen.com/static/5fc3f1e0a9af60c718c16fb7262b0ec1/a987b/jarednielsen-javascript-array-data-structure-example.png)

**Down below is an example of array:**




> colors= ['white',


> 'black',


> 'custom']; 

















