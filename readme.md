# CSS Position Properties

![cover](https://user-images.githubusercontent.com/110910838/206276245-f4d7efe5-148c-4d60-9a2b-cb1ec158c9d0.png)

In this article we are going to walk

# What is CSS Position property? 🤔

The position properties determine where the element should be located in the document. You can place your element anywhere you wish using CSS properties and can create beautiful, stunning, artistic and unique asymmetrical websites.

Here is an example, 👇

![image1](https://user-images.githubusercontent.com/110910838/206276707-46a3e693-008d-4db2-9804-79ec41736795.png)
Using position properties, you can move those flowers, images, and patterns all around the page.

There are 5 values for the position property

Static

Relative

Absolute

Fixed

Sticky

# Static

This is a default value. Static-positioned elements are not affected by the top, bottom, right, left, and z-index properties. This has no use cases.

Project Setup

Let's create the setup for our learning with some HTML and CSS
```html
<div class="parent">Parent element
    <div class="child">Child element</div>
</div>
```
```css
body, html{
    height: 100%;
    font-family: sans-serif;
}
body{
    display: flex;
    justify-content: center;
    align-items: center;
}
.parent{
    border: 2px solid #dc143c;
    color:#dc143c;
    padding:40px;
    text-align: center;

}
.child{
    border:1px solid #0051ff;
    color:#0051ff;;
    padding:20px;
    background-color: #eee;
    margin-top: 10px;
}
```
The output is 👇
![pos1](https://user-images.githubusercontent.com/110910838/206280209-3eaabc5f-3a8e-4666-9fd1-14e72fc51c39.png)

To move our child element we can use four properties top, bottom, left, and right after giving it position properties. Let's try with relative value

# Relative
```css
.child{
position: relative;
top: 80px;
left:80px
}
```
The output is 👇
![pos2](https://user-images.githubusercontent.com/110910838/206276730-7e342dee-3d5b-453e-8c0c-c551f069fac5.png)

The element is positioned relative to its normal position and offsets relative to itself based on the value we have given so here the child element now moved down by 80px and right by 80px

The offset does not affect the position of any other elements.

What about Absolute 🤔

# Absolute
```css
.child{
position: absolute;
}
```
The output looks like this 👇
![pos3](https://user-images.githubusercontent.com/110910838/206276735-3da082ee-546e-4248-879e-4f1bf82ece9b.png)
If the child element is given an absolute value, then the parent element will behave as if the child isn't there at all. And when we set other values such as top, bottom, left, and right, we can see the child element is responding not to the dimension of its parents, but to the document.

Here is an example 👇
```css
.child{
position: absolute;
top: 50px;
left:0px;
}
```
The output looks like this 👇
![pos4](https://user-images.githubusercontent.com/110910838/206276746-71e631cf-1262-4383-8048-c54a9fe42925.png)

