# Grid
- **CSS Grid Layout, often referred to simply as Grid, is a two-dimensional layout system in CSS that allows you to design complex web layouts with rows and columns. It provides a highly flexible and precise way to arrange and align content on a webpage.**

#### 1)Two-Dimensional Grid: */

- **Unlike traditional layout models, such as the box model and Flexbox, CSS Grid is a two-dimensional layout system. It simultaneously manages both rows and columns.**

#### 2)Grid Container and Grid Items

- **A grid layout consists of a grid container and its grid items.**
- **The grid container is an element that contains grid items. It's often an immediate parent element.**
- **Grid items are the children of the grid container, and they are positioned within the grid.**

#### 3) Defining the Grid
- **To create a grid, you first define the columns and rows.**
- **Use the grid-template-columns and grid-template-rows properties to set the sizes and structure of the grid.**
- **Columns and rows can be specified as fixed sizes (e.g., pixels) or flexible sizes (e.g., percentages, fractions).**
## Example-1(display: grid; grid-template-rows: 250px 250px;)
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  /* grid starts here  */
  display: grid;
  grid-template-rows: 250px 250px;
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}

```
### Output
![image](https://github.com/user-attachments/assets/cc0d9027-2d83-4feb-bac5-662bf3e3f4df)
## Example-2(display: grid; grid-template-rows: 250px 250px;grid-template-columns: 250px 250px 1fr;)
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  /* grid starts here  */
  display: grid;
  grid-template-rows: 250px 250px;
  grid-template-columns: 250px 250px 1fr;
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}

```
### Output
![image](https://github.com/user-attachments/assets/c2ec09eb-26e2-4cff-ab6e-1336383296b3)
## Example-3(display: grid;grid-template-rows: 250px 250px;grid-template-columns: 1fr 1fr 1fr;)
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  /* grid starts here  */
  display: grid;
  grid-template-rows: 250px 250px;
  grid-template-columns: 1fr 1fr 1fr;
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}

```
### Output
![image](https://github.com/user-attachments/assets/47d0ba76-85cb-490d-b509-7a85486517c4)
## Example-3( display: grid;grid-template-rows: repeat(2,250px);grid-template-columns: repeat(3,1fr);)
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  /* grid starts here  */
   display: grid;
  grid-template-rows: repeat(2,250px);
  grid-template-columns: repeat(3,1fr);
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}

```
### Output
![image](https://github.com/user-attachments/assets/dbbd4e66-7c51-430d-b13c-c4743f3b4521)

#### 4)Grid Lines and Tracks:
- **Grid lines are the dividing lines between columns and rows.**
- **Tracks are the spaces between grid lines where content can be placed.**
- **You can name grid lines and tracks for better organization.**

![image](https://github.com/user-attachments/assets/26f2ce7b-a584-4aa8-b675-ce3580b2c803)

#### 5)Placing Grid Items: 
- **Grid items are placed within the grid using the ```grid-column``` and ```grid-row``` properties.**
- **We can also use the shorthand property ```grid-area``` to specify both column and row placement in a single declaration.**
- **The grid-area property specifies a grid item's size and location in a grid layout, and is a shorthand property for the following properties**
- **```grid-area:grid-row-start/grid-column-start/grid-row-end/grid-column-end```**
### Example-1 ```grid-column``` and ```grid-row```
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <!-- <div class="item item-2">item-2, World Best CSS CourseEver</div> -->
      <!-- World Best CSS CourseEver -->
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
display: grid;
grid-template-rows: repeat(2,250px);
grid-template-columns: repeat(3,1fr);
gap: 50px; 
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
  grid-row-start: 2;
  grid-row-end: 3;
/*shortened of grid-row-start and grid-row-end is grid-row */
  /* grid-row: 2 / 3; */
  grid-column-start: 2;
  grid-column-end: 3;
/*shortened of grid-column-start and grid-column-end is grid-column */
  /* grid-column: 2 / 3; */
/*grid-area:grid-row-start/grid-column-start/grid-row-end/grid-column-end*/
  /* grid-area: 2 / 2 / 3 / 3; */
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}
```
### Output
![image](https://github.com/user-attachments/assets/cb98c842-0c9c-47e0-99a4-f9731057efb2)
### Example-1 ```grid-column``` and ```grid-row``` and ```grid-area```
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <!-- <div class="item item-2">item-2, World Best CSS CourseEver</div> -->
      <!-- World Best CSS CourseEver -->
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
display: grid;
grid-template-rows: repeat(2,250px);
grid-template-columns: repeat(3,1fr);
gap: 50px; 
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
  /*grid-row-start: 2;
  grid-row-end: 3;*/
/*shortened of grid-row-start and grid-row-end is grid-row */
  /* grid-row: 2 / 3; */
  /* grid-column-start: 2;
  grid-column-end: 3; */
/*shortened of grid-column-start and grid-column-end is grid-column */
  /* grid-column: 2 / 3; */
/*grid-area:grid-row-start/grid-column-start/grid-row-end/grid-column-end*/
   grid-area: 2 / 2 / 3 / 3; 
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
   grid-row: 1/2;
  grid-column: 2/4;
/*we can use grid-area instead of grid-row and grid-column*/
grid-area:1/2/2/4;
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}
```
### Output
![image](https://github.com/user-attachments/assets/9b331a46-9505-4485-83cd-f884124ba153)
### 6)Grid Gaps
- **Grid gaps are the spaces between grid items and tracks.**
- **You can control gaps between columns and rows separately using the grid-column-gap and grid-row-gap properties or the shorthand grid-gap.**
- **This property is a shorthand for the following CSS properties: The gap CSS shorthand property sets the gaps (gutters) between rows and columns.**
## grid-column-gap,grid-row-gap(deprecated)
### Example-1(grid-row-gap: 50px; grid-column-gap: 50px;)
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  /* grid starts here  */
   display: grid;
  grid-template-rows: repeat(2,250px);
  grid-template-columns: repeat(3,1fr);
  grid-row-gap: 50px; /*deprecated*/
  grid-column-gap: 50px;/*deprecated*/
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}

```
### Output
![image](https://github.com/user-attachments/assets/0d40f5f8-de49-4895-9232-fcd8325f6a8a)
## grid-gap(deprecated)
### Example-2(grid-gap: 50px;)-->deprecated
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  /* grid starts here  */
   display: grid;
   grid-template-rows: repeat(2,250px);
   grid-template-columns: repeat(3,1fr);
   grid-gap: 50px;
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}
```
### Output
![image](https://github.com/user-attachments/assets/236fd78d-72cb-4c0a-a1a8-b4da621f3b2e)
## Example-3(row-gap;column-gap)/gap;-->Updated
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <div class="item item-3--child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  /* grid starts here  */
   display: grid;
grid-template-rows: repeat(2,250px);
grid-template-columns: repeat(3,1fr);
row-gap: 50px; 
column-gap:50px;
/*instead of row-gap and column-gap we can use gap only*/
/*gap:50px;*/
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}

```
### Output
![image](https://github.com/user-attachments/assets/a08c1cd9-4ba0-4f1c-b17f-9da05a2b6771)
# Explicit vs Implicit grid
- **Sometimes we created some layout that we did not create explicitly but some grid sections were created implicitly. Like below example item-6.**
- **In this case we use ```grid-auto-rows``` and ```grid-auto-columns```**

![image](https://github.com/user-attachments/assets/9b331a46-9505-4485-83cd-f884124ba153)

### 7)Grid Auto:
- **Grid items can be automatically placed using grid-auto-flow. By default, they fill rows, but you can change this behavior to fill columns.**
- **grid-auto-rows and grid-auto-columns control the size of automatically placed items.**
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <!-- <div class="item item-2">item-2, World Best CSS CourseEver</div> -->
      <!-- World Best CSS CourseEver -->
      <div class="item item-3 child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
/* Example of grid-auto-rows to main implicit grid*/
display: grid;
grid-template-rows: repeat(2,250px);
grid-template-columns: repeat(3,1fr);
grid-auto-rows:250px ;
gap: 50px;
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
/* we can change the positions easily  */
.item-1 {
  background-color: #662549;
  /* grid-row-start: 2;
  grid-row-end: 3; */
/*shortened of grid-row-start and grid-row-end is grid-row */
  /* grid-row: 2 / 3; */
  /* grid-column-start: 2;
  grid-column-end: 3; */
/*shortened of grid-column-start and grid-column-end is grid-column */
  /* grid-column: 2 / 3; */
/*grid-area:grid-row-start/grid-column-start/grid-row-end/grid-column-end*/
grid-area: 2 / 2 / 3 / 3;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
  /* grid-row: 1/2;
  grid-column: 2/4; */
  /*we can use grid-area instead of grid-row and grid-column*/
  grid-area:1/2/2/4;
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}
```
### Output
![image](https://github.com/user-attachments/assets/f5655128-139b-43ba-8622-a9ebaf5e9dae)

# 9) Alignment and Justification:
- **You can align and justify content within grid items and the grid container itself.**
- **Properties like justify-items, align-items, justify-content, and align-content help you control alignment and spacing.**
### Example:align-items: self-start;
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <!-- <div class="item item-2">item-2, World Best CSS CourseEver</div> -->
      <!-- World Best CSS CourseEver -->
      <div class="item item-3 child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  display: grid;
grid-template-rows: repeat(2,250px);
grid-template-columns: repeat(3,1fr);
grid-auto-rows:250px ;
gap: 50px; 
  /* align-items: center; */
  align-items: self-start;
  /* align-items: self-end; */
  /* align-items: stretch; */
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}
```
### Output
![image](https://github.com/user-attachments/assets/f1c86b59-5762-433e-809e-8c21868e824a)
### Example:align-items: self-end;
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <!-- <div class="item item-2">item-2, World Best CSS CourseEver</div> -->
      <!-- World Best CSS CourseEver -->
      <div class="item item-3 child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  display: grid;
grid-template-rows: repeat(2,250px);
grid-template-columns: repeat(3,1fr);
grid-auto-rows:250px ;
gap: 50px; 
  /* align-items: center; */
  /*align-items: self-start;*/
  align-items: self-end;
  /* align-items: stretch; */
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}
```
### Output
![image](https://github.com/user-attachments/assets/a1eddeee-07a3-465f-aa85-1e8ff081eaaa)
### Example:align-items: center;
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <!-- <div class="item item-2">item-2, World Best CSS CourseEver</div> -->
      <!-- World Best CSS CourseEver -->
      <div class="item item-3 child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  display: grid;
grid-template-rows: repeat(2,250px);
grid-template-columns: repeat(3,1fr);
grid-auto-rows:250px ;
gap: 50px; 
   align-items: center; 
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}
```
### Output
![image](https://github.com/user-attachments/assets/fad99600-62d0-48f4-9ea5-f1af5a8108d4)
### Example:align-items: stretch;
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Grid</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="grid-container">
      <div class="item item-1">item-1</div>
      <div class="item item-2">item-2</div>
      <!-- <div class="item item-2">item-2, World Best CSS CourseEver</div> -->
      <!-- World Best CSS CourseEver -->
      <div class="item item-3 child">item-3</div>
      <div class="item item-4">item-4</div>
      <div class="item item-5">item-5</div>
      <div class="item item-6">item-6</div>
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
body {
  min-height: 100vh;
  background-color: #2c3639;
}
.grid-container {
  width: 80%;
  margin: 100px auto;
  background-color: #dcd7c9;
  color: #fff;
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  display: grid;
grid-template-rows: repeat(2,250px);
grid-template-columns: repeat(3,1fr);
grid-auto-rows:250px ;
gap: 50px; 
align-items: stretch; 
}
.item {
  display: grid;
  place-items: center;
  text-transform: uppercase;
  font-size: 20px;
  letter-spacing: 2px;
  font-weight: bold;
}
.item-1 {
  background-color: #662549;
}
.item-2 {
  background-color: #113946;
}
.item-3 {
  background-color: #102c57;
}
.item-4 {
  background-color: #884a39;
}
.item-5 {
  background-color: #454545;
}
.item-6 {
  background-color: #85586f;
}
```
### Output
![image](https://github.com/user-attachments/assets/b7375189-84fb-4845-8e8c-bd2772e7d6e4)

/*? 8. Responsive Grids: */

/* CSS Grid is highly responsive. Grid items can be repositioned and resized automatically as the viewport size changes. */
/* Use media queries to adjust grid layouts for different screen sizes. */


