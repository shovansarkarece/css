# FLEXBOX IN CSS
- **Flexbox is a one-dimensional layout model that helps you distribute space along a single axis (either horizontally or vertically) in a flexible and efficient way. It allows you to align and distribute elements within a container, making it easier to create complex layouts without using floats or positioning.**
# Flex Container Properties (Parent) 
![image](https://github.com/user-attachments/assets/b2ccb40a-d802-4396-9c98-86968708f233)

- **1)Flex Container (display: flex;):**
- **To create a flexbox layout, you need a flex container. Apply display: flex; to the container element.**
- **display:flex always apply on parent not apply in children**
- Syantax:
```
.flex-container {
     display: flex;
}
```
#### Example-1(display: flex;)
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Flexbox CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1 id="main-heading">CSS FlexBox (Flexible Box Layout)</h1>
    <hr />
    <br />
    <section class="flex-container">
      <div class="item item-1">item 1</div>
      <div class="item item-2">item 2</div>
      <div class="item item-3">item 3</div>
      <div class="item item-4">item 4</div>
    </section>
  </body>
</html>
/*style.css*/
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html {
  font-size: 62.5%;
  font-family: "Urbanist", sans-serif;
}

body {
  display: grid;
  place-items: center;
  background-color: hsl(0, 0%, 96%);
}

#main-heading {
  font-size: 6.2rem;
  color: #1e1403;
  margin: 3rem 0;
}

.flex-container {
  width: 60%;
  height: 600px;
}
.flex-container {
/* when we use 
disply:flex,
flex-direction: row;
flex-direction: row-reverse; 
flex-direction:column;
flex-direction: column-reverse;
then uncomment below code*/
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
flex-direction: row;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
### Output:
![image](https://github.com/user-attachments/assets/87653346-fb42-49f6-83fe-d4f34c847463)


# Graphical representation of main axis vs cross axis
- **Main Axis and Cross Axis:**
- **In a flex container, one axis is considered the main axis, and the other is the cross axis. You can set the main axis to be either horizontal (row) or vertical (column).**

![image](https://github.com/user-attachments/assets/14ca2d2f-90fc-4e0a-b955-8c8cf8fc1708)

- **2)Flex Direction (flex-direction): Use flex-direction to specify the direction to either main axis or cross-axis.**
![image](https://github.com/user-attachments/assets/6f10ec3b-c695-4ac9-a376-b5e717b80994)

- **Values: row, row-reverse, column, column-reverse.**
- **Items display in a row (the flex-direction property's default is row).**
- **If the flex-direction:row then horizontal will be main-axis.** 
- **if flex-direction:column the vertical part will be main-axis and horizontal axis become the cross axis.**
- **flex-direction: row | row-reverse | column | column-reverse; always apply to parent not to children**
- Syntax:
```
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```
- **flex-direction:column**

![image](https://github.com/user-attachments/assets/d4697a3c-70ab-4cf6-8134-7a8a681213bc)
- **3)Justify Content (justify-content): justify-content aligns flex items along the main axis means horizontally.**
- **Values include flex-start, flex-end, center, space-between, and space-around.**
- **justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly; always apply to parent not to children**

![image](https://github.com/user-attachments/assets/35b7c9d2-4eae-4ad3-8b34-63f2a3d4d406)
- **Syntax:**
```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
}
```
#### Example
- **justify-content: flex-start/start**
 
![image](https://github.com/user-attachments/assets/01703b19-fec1-42cc-b26a-d0df40747f2c)
- **justify-content: center**

![image](https://github.com/user-attachments/assets/dcdf37f9-4d84-4e3d-b13f-3be72105ec7a)
- **justify-content: flex-end/end**

![image](https://github.com/user-attachments/assets/03ee4d59-c85f-4d1a-9916-94f5d3ce8556)
- **justify-content:space-between**
  
![image](https://github.com/user-attachments/assets/b99bd807-df24-4333-b3e0-f7dec0721155)

- **4)Align Items (align-items):**
- **align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start ; always apply to parent not to children**

![image](https://github.com/user-attachments/assets/50d551c1-bc0f-40d1-9840-850f32a56beb)
- **Syntax:**
```
.container {
  align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start ;
}
```
- **align-items align flex items along the cross-axis means vertically.**
- **Values include flex-start, flex-end, center, stretch, and baseline.**

- **align-items: start**

![image](https://github.com/user-attachments/assets/c4552ff8-d36b-490f-a813-4a5a3a8dd5b6)

- **align-items: end**

![image](https://github.com/user-attachments/assets/07a62c3a-5e14-4b46-8ed7-ec0d69fbb993)

- **align-items: center**

![image](https://github.com/user-attachments/assets/32fab510-ec93-47f5-9bfc-0ce2df76c9d8)

- **1: How do you center a div or text both horizontally and vertically using Flexbox? ⭐⭐⭐⭐⭐**
- **To center items horizontally, you can use justify-content: center; on the flex container.**
- **To center items vertically, you can use align-items: center; on the flex container.**
- **We can use both ```justify-content: center;align-items: center;``` to center any element horizontally and vertically.**
 
![image](https://github.com/user-attachments/assets/189becd8-e757-4d51-a1ce-caef1115baad)

- **5) flex-wrap:**
- **Specifies whether flex items should wrap to the next line when they overflow the container.**
- **By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.**
- **Values: nowrap (default), wrap, wrap-reverse.**
- **nowrap (default): all flex items will be on one line**
- **wrap: flex items will wrap onto multiple lines, from top to bottom.**
- **wrap-reverse: flex items will wrap onto multiple lines from bottom to top.**
- **flex-wrap: nowrap | wrap | wrap-reverse; always apply to parent not to children.**
- **Syntax:**
```
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

![image](https://github.com/user-attachments/assets/76798933-449f-4da3-9822-4ff18af0b8c8)

- **6) align-content:**
- **We can only use align-content when we specifically use flex-wrap, neither it is impossible to use.** 
- **Aligns multiple lines of flex items when there is extra space along the cross axis.**
- **Values: flex-start, flex-end, center, space-between, space-around, stretch.**
- **align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end ; always apply to parent not to children.**
- **Syntax:**
```
.container {
  align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end ;
}
```
![image](https://github.com/user-attachments/assets/3c4ed7ae-515c-4f9f-888e-d5a73a79e82a)

#### Above all property applied on parent but below properties will be applied in children only.
/** ------------- Flex Item Properties (children) ------------ */
/*? a. order:
- Determines the order in which a flex item appears relative to other flex items within the container.
- Lower values come first. */

/*? b. flex-grow:
- Specifies how much a flex item should grow to fill available space along the main axis.
- Default value is 0, meaning it won't grow. */

/*? c. flex-shrink:
- Specifies how much a flex item should shrink when there isn't enough space along the main axis.
- Default value is 1, meaning it will shrink. */

/*? d. flex-basis:
- Defines the initial size of a flex item along the main axis.
- Default value is auto, which means the item's size is determined by its content. */

/*? e. flex (Shorthand for flex-grow, flex-shrink, and flex-basis):
- Combines the three flex item properties in one declaration. */

/** ---------- Alignment Properties (Self) ---------------- */

/*? a. align-self:
- Overrides the align-items property for an individual flex item.
- Allows you to align a single item differently from others. */
