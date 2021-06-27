## Domain Modeling

***Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.***

***A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.***

## Tables

![Table](https://cdn.educba.com/academy/wp-content/uploads/2019/10/Create-Tables-in-HTML.png)

### What's a Table?

***A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.***

**There are several types of information that need to be displayed in a grid or table. For example: sports results, stock reports, train timetables.**


### Basic Table Structure

> `<table>` : The `<table>` element is used to create a table. The contents of the table are written out row by row.


> `<tr>`: You indicate the start of each row using the opening `<tr>` tag. (The tr stands for table row.) It is followed by one or more `<td>` elements (one for each cell in that row). At the end of the row you use a closing `</tr>` tag.

> `<td>`: Each cell of a table is represented using a `<td>` element. (The td stands for table data.) At the end of each cell you use a closing `</td>` tag.

### Table headings

`<th>` : The `<th>` element is used just like the `<td>` element but its purpose is to represent the heading for either a column or a row. (The the stands for table heading.) Even if a cell has no content, you should still use a `<td>` or `<th>` element to represent the presence of an empty cell otherwise the table will not render correctly. (The first cell in the first row of this example shows an empty cell.)


## Creating an Object : Constructor Notation 

![createanobject](https://miro.medium.com/max/560/1*DnOmZR328jCXUAXjR6-Alg.jpeg)

***the new keyword and the object constructor create a blank object. you can then add properties and methods to the Object.***


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


### Updating an object 

**This is an example of Updating an Object**

`hotel.name='park';`



### CREATING MANY OBJECTS: CONSTRUCTOR NOTATION 


![constructor](https://miro.medium.com/max/4096/1*KYFTHD69xtacnwbKRyFuqQ.png)


***Sometimes you will want several objects to represent similar things. Object constructors can use a function as a template for creating objects. First, create the template with the object's properties and methods.***

***you create instances of the object using the constructor function.the new keyword followed by a call to the function creates a new object. the properties of each object are given as arguments to the function.***


>`var quayHotel=new hotel('quay',40,25);`


>`var quayHotel=new hotel('quay',40,25);`







