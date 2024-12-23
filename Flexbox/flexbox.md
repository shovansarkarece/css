# FLEXBOX IN CSS
- **Flexbox is a one-dimensional layout model that helps you distribute space along a single axis (either horizontally or vertically) in a flexible and efficient way. It allows you to align and distribute elements within a container, making it easier to create complex layouts without using floats or positioning.**
# Flex Container Properties (Parent) 
![image](https://github.com/user-attachments/assets/b2ccb40a-d802-4396-9c98-86968708f233)

#### 1)Flex Container (display: flex;):
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
#### Output:
![image](https://github.com/user-attachments/assets/87653346-fb42-49f6-83fe-d4f34c847463)


#### Graphical representation of main axis vs cross axis
- **Main Axis and Cross Axis:**
- **In a flex container, one axis is considered the main axis, and the other is the cross axis. You can set the main axis to be either horizontal (row) or vertical (column).**

![image](https://github.com/user-attachments/assets/14ca2d2f-90fc-4e0a-b955-8c8cf8fc1708)

#### 2)Flex Direction (flex-direction): Use flex-direction to specify the direction to either main axis or cross-axis.
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
#### flex-direction:column**

![image](https://github.com/user-attachments/assets/d4697a3c-70ab-4cf6-8134-7a8a681213bc)

#### Example-1(display: flex;flex-direction: row;)
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
#### Output:
![image](https://github.com/user-attachments/assets/428346eb-9a82-4379-bdeb-bc065486c58f)
#### Example-2(display: flex;flex-direction: row-reverse;)
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
flex-direction: row-reverse;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/ef6f1c69-f94c-439f-a324-2330a1c4f3cc)
#### Example-3(display: flex;flex-direction:column;)
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
flex-direction: column;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/dcfe3de4-2f78-48ad-97f4-0432b9e6df3f)
#### Example-4(display:flex;flex-direction:column-reverse;)
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
flex-direction:column-reverse;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/4d06a021-eb7e-4e68-9e07-576144fbc8a4)

#### 3)Justify Content (justify-content): justify-content aligns flex items along the main axis means horizontally.
- **Values include flex-start, flex-end, center, space-between, and space-around.**
- **justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly; always apply to parent not to children**
### justify-content: center; always works horizontally when we are using flex-direction: row; and if we use flex-direction: column; then it will be working vertically.

![image](https://github.com/user-attachments/assets/35b7c9d2-4eae-4ad3-8b34-63f2a3d4d406)
- **Syntax:**
```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
}
```
![image](https://github.com/user-attachments/assets/01703b19-fec1-42cc-b26a-d0df40747f2c)
#### Example-1(display: flex; justify-content: flex-start;)-->flex-start and start both are same
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
 justify-content: flex-start;/*flex-start and start both are same*/
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/dd98c9d0-38ce-4fa8-8a12-180a7b567a53)

#### justify-content:center

![image](https://github.com/user-attachments/assets/dcdf37f9-4d84-4e3d-b13f-3be72105ec7a)

#### Example-2(display: flex;justify-content: center;)
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
 justify-content: center;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/a1268d75-1167-4bcc-b22c-2ff50910366b)

#### justify-content: flex-end/end
![image](https://github.com/user-attachments/assets/03ee4d59-c85f-4d1a-9916-94f5d3ce8556)
#### Example-3(display: flex; justify-content: flex-end;)-->flex-end and end both are same
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
 justify-content: flex-end;/*flex-end and end both are same*/
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/a177de13-d880-415d-acfd-d9a56974f15f)

#### justify-content:space-between
  
![image](https://github.com/user-attachments/assets/b99bd807-df24-4333-b3e0-f7dec0721155)

#### Example-4(display: flex;justify-content:space-between;)
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
 justify-content: space-between;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/0aef0e23-7430-4163-9798-fd9338fe4ec0)
#### justify-content:space-evenly
![image](https://github.com/user-attachments/assets/0280dbce-f045-4d81-afba-7db6eac53d9b)
#### Example-4(display: flex;justify-content:space-evenly;)
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
 justify-content: space-evenly;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/97d5ec81-c047-448b-bd1c-c26477325854)


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

### 5) flex-wrap:**
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
- **This property only takes effect on multi-line flexible containers, where flex-wrap is set to either wrap or wrap-reverse).**
- **Values: flex-start, flex-end, center, space-between, space-around, stretch.**
- **align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end ; always apply to parent not to children.**
- **Syntax:**
```
.container {
  align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end ;
}
```
![image](https://github.com/user-attachments/assets/3c4ed7ae-515c-4f9f-888e-d5a73a79e82a)

## Above all property applied on parent but below properties will be applied in children only.
# Flex Item Properties (children)
#### a)order:
- **Determines the order in which a flex item appears relative to other flex items within the container.**
- **Lower values come first.**
#### Example:order
![image](https://github.com/user-attachments/assets/2767a23a-6a3f-4d9c-a350-2dc3f5454d8e)

#### b)flex-grow:

![image](https://github.com/user-attachments/assets/fa265a73-0b8a-4b89-b377-bbff9a6176de)

- **Specifies how much a flex item should grow to fill available space along the main axis.**
- **Default value is 0, meaning it won't grow.**
- - **Negative numbers are invalid.**
- **This defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion.**
- **If all items have flex-grow set to 1, the remaining space in the container will be distributed equally to all children.**
#### Example-flex-grow
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
flex-direction: row;
 justify-content: start;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
.item-2 {
  flex-grow: 1;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/fd3218a9-6ff9-4d73-8383-36733eb9b8af)
#### Example-flex-grow
![image](https://github.com/user-attachments/assets/961e0f0c-4d24-49d5-bf89-d6363131d3cd)
#### c)flex-shrink:
- **Specifies how much a flex item should shrink when there isn't enough space along the main axis.**
- **Default value is 1, meaning it will shrink.**
- **This defines the ability for a flex item to shrink if necessary.**
- **Syntax**
```
.item {
  flex-shrink: 3; /* default 1 */
}
```
#### Example-flex-shrink
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
flex-direction: row;
 justify-content: start;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
.item-2 {
  flex-grow: 1;
  flex-shrink: 5;
}
```
#### Output:
![image](https://github.com/user-attachments/assets/6ecee2df-c5ff-4e5d-a511-988de6aaca5a)
### Example:flex-shrink
![image](https://github.com/user-attachments/assets/c3630b20-4e83-487c-8446-765bc0b6393d)

#### d) flex-basis:

![image](https://github.com/user-attachments/assets/d40a8de9-4b01-4fb9-b842-d5fbd5570972)
- **Defines the initial size of a flex item along the main axis.**
- **Default value is auto, which means the item's size is determined by its content.**
- **This defines the default size of an element before the remaining space is distributed. It can be a length (e.g. 20%, 5rem, etc.)**
- **Syntax**
```
.item {
  flex-basis:  | auto; /* default auto */
}
```
#### Example-flex-basis
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
flex-direction: row;
 justify-content: start;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
.item-3 {
  flex-basis: 200px;
}
```
#### Output
![image](https://github.com/user-attachments/assets/48717248-a438-4a2b-ae53-93680f40c736)
### Example-without flex-basis
![image](https://github.com/user-attachments/assets/b94a28ed-030f-4010-a552-a470ff6953ce)

### Example-flex-basis
![image](https://github.com/user-attachments/assets/bcfa289a-09e9-4644-ab92-04d911628c3a)


#### e)align-self:
- **Overrides the align-items property for an individual flex item.**
- **Allows you to align a single item differently from others.**
- **Syantax**
```
item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```
#### Example-align-self
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
  width: 60%;
  height: 600px;
  margin: 0 auto;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  background: linear-gradient(to right, #514a9d, #24c6dc);
  color: #fff;
  /* flexbox container properties */
  display: flex;
flex-direction: row;
 justify-content: start;
.item{
  width: 100px;
  height: 100px;
  background-image: linear-gradient(to right top, #004d7a, #00bf72, #a8eb12);
  box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px, rgb(51, 51, 51) 0px 0px 0px 3px;
  font-size: 24px;
}
.item-2 {
  align-self: center;
}
```
#### Output
![image](https://github.com/user-attachments/assets/231d651e-6f05-483d-ba8b-f7fa506b9097)


### e)flex (Shorthand for flex-grow, flex-shrink, and flex-basis):
- **This is the shorthand for flex-grow, flex-shrink and flex-basis combined.**
- **The second and third parameters (flex-shrink and flex-basis) are optional.**
- **The default is 0 1 auto, but if you set it with a single number value, like flex: 5;, that changes the flex-basis to 0%, so it’s like setting flex-grow: 5; flex-shrink: 1; flex-basis: 0%;.**
- **Syntax:**
```
.item {
  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
}
```
