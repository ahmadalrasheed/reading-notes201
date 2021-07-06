## HTML & CSS

### Transforms

![transforms](https://miro.medium.com/max/900/1*_6MfwckxNfQTca9SiG8MdQ.png)

***With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.***

***The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.***

***Within this lesson we’ll take a look at both two-dimensional and three-dimensional transforms. Generally speaking, browser support for the transform property isn’t great, but it is getting better every day. For the best support vendor prefixes are encouraged, however you may need to download the nightly version of Chrome to see all of these transforms in action.***


### Transform Syntax

***The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.***

>div {
-webkit-transform: scale(1.5);
-moz-transform: scale(1.5);
-o-transform: scale(1.5);
transform: scale(1.5);
}



## Transitions & Animations

![transitions](https://i1.wp.com/www.cssscript.com/wp-content/uploads/2021/01/40-CSS-Transitions-For-Entrance-Exit-Animations-transition.css.png?fit=738%2C512&ssl=1)

***One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.***

***With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.***

***Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.***

**In the example below the box will change its background color over the course of 1 second in a linear fashion.** 



>.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}

              
### Amazing simple CSS transitions


***All of these effects (bar one) are controlled with the transition property. So we can see these effects working, we’ll set up a div in an HTML page:***

> `<!DOCTYPE html>`
 `<html>`
`<head>`
   ` <style type="text/css">`
    `</style>`
`</head>`
`<body>`
    `<div></div>`
`</body>`
`</html>`

***Having done so, set its width and height (so it has dimensions), its background color (so we can see it) and its transition property.***

`<style type="text/css">`
`body > div`
`{`
            `width:483px;`
           ` height:298px;`
           ` background:#676470;`
           ` transition:all 0.3s ease;`
`}`
`</style>`

***The transition property has three values: the properties to transition (in our case all of them) the speed of the transition (in our case 0.3 seconds) and a third value which lets you change how the acceleration and deceleration is calculated, but we’ll stick with the default by leaving this blank.***

***Now all we need to do is change properties, and they’ll animate for us…***

![animation](https://res.cloudinary.com/practicaldev/image/fetch/s--GZYZPBSr--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://res.cloudinary.com/practicaldev/image/fetch/s--HLCG8XKx--/c_imagga_scale%2Cf_auto%2Cfl_progressive%2Ch_720%2Cq_auto%2Cw_1280/https://dev-to-uploads.s3.amazonaws.com/i/54ydb37tzyny06ac8xdf.jpg)

* **Fade in**
Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.


    Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover:

>.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}

* **Change color**
Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS:

>.color:hover
{
        background:#53a7ea;
}

* **Rotate elements**
CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS:


>.rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}
