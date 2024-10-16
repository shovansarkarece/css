## transform: translate()
- **The translate() function is used to move an element along the X and Y axes within its containing block.**
- **It takes two values: one for horizontal translation (X-axis) and one for vertical translation (Y-axis).**
## translate(x, y) - Moves the element by x units horizontally and y units vertically.
#### Example-1:transform: translateX();
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}
.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
  transform: translateX(500px);
}
```
#### Output
https://github.com/user-attachments/assets/f801376b-0ec5-45e5-ac59-fa6654020eed
#### Example-2:transform: translateY();
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}

.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
transform: translateY(500px); 
  translate: 0 500px;
}
```
#### Output
https://github.com/user-attachments/assets/067b247a-efcf-416a-83db-6a5b6b575a70
#### Example-3: translate();
- **Here first parameter will be X axis value and 2nd parameter will be Y axis value.** 
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}

.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
  translate: 0 500px;
}
```
#### Output
https://github.com/user-attachments/assets/067b247a-efcf-416a-83db-6a5b6b575a70
#### Example-1:translate();
- **Here first parameter will be X axis value and 2nd parameter will be Y axis value.** 
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}
.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
  translate: 500px 0;
```
#### Output
https://github.com/user-attachments/assets/f801376b-0ec5-45e5-ac59-fa6654020eed
#### Example-2:translate();
- **Here first parameter will be X axis value and 2nd parameter will be Y axis value.** 
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}
.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
  translate: 500px 200px;
}
```
#### Output
https://github.com/user-attachments/assets/be788dac-625b-40c7-8ad9-da60fba178e2
## transform: scale()
- **The scale() function takes one or two values**
- **scale(x) - Scales the element by a factor of x along both the X and Y axes. A value of 1 is the original size, values greater than 1 make it larger, and values less than 1 make it smaller.**
- **scale(x, y) - Scales the element by a factor of x along the X-axis and y along the Y-axis. You can use different values for horizontal and vertical scaling.**
#### Example-2: scale: 0.5; or we can use transform: scale(2); */
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}
.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
  scale: 0.5;
   /* transform: scale(2); */
    /* transform: scaleX(0.5); */
 /* transform: scaleY(2);  */
}
```
#### Output
https://github.com/user-attachments/assets/8e226d4c-64d6-4646-aa87-7cb9c694ef84


## transform: rotate()
- **The rotate() function takes one parameter**
## rotate(angle) - Specifies the angle of rotation in degrees. Positive values rotate clockwise, and negative values rotate counterclockwise. */
### Example-2: transform: rotateX(45deg); 
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}
.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
  transform: rotate(90deg); 
  /* transform: rotate(180deg); */
  /* transform: rotateX(180deg); */
   /* transform: rotateY(180deg); */
   /* transform: rotateX(45deg);
}
```
#### Output
https://github.com/user-attachments/assets/58e3a4d8-dbdb-4a1c-8182-f91774ab4842





## skew() method skews an element along the X and Y-axis by the given angles.
- **We can use this to create visually interesting effects, such as tilting or slanting elements.**
### Example-1: transform: skew(20deg);
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}
.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
transform: skew(20deg);  
   /* transform: skewX(-20deg); */
    /* transform: skewY(-20deg); */
}
```
#### Output
https://github.com/user-attachments/assets/c84c21ce-f7ba-4a5f-ba5c-dfc47cd88810



# transform-origin with rotate

>The transform-origin property in CSS allows you to specify the point around which a transformation should occur.
>>It determines the origin point for transformation functions like rotate, scale, skew, and translate.
>>>Understanding how transform-origin works is crucial for controlling the position and behavior of transformed elements.
### Example-1:rotate: -20deg;transform-origin: left; transform-origin: right;
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <!-- <div class="box">translate</div> -->
      <!-- <div class="box">scale</div> -->
      <!-- <div class="box">Rotate</div> -->
      <!-- <div class="box">skew</div> -->
      <!-- <div class="box">img</div> -->
      <img class="box" src="../../images/html.png" alt="" srcset="" />
    </div>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Urbanist", sans-serif;
}

body {
  background-color: hsl(0, 0%, 85%);
  background-color: #2b3033;
}

.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  box-shadow: inset 0 0 0 5px #4861ec;
}
.box {
  /* width: 250px;
    height: 100px; */
  /* below three properties for scale and transform */
  width: 250px;
  height: 250px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 20px;
  color: #fff;
  font-size: 2rem;
  text-transform: capitalize;
  display: flex;
  justify-content: center;
  align-items: center;
  transition-property: all;
}
.container img {
  width: 100%;
  width: 30%;
  height: auto;
  transition: all 1s linear;
}
.container img:hover {
     rotate: -20deg;
rotate: 20deg;
  transform-origin: left;
 /*transform-origin: right;  */ 
}
```
#### Output
https://github.com/user-attachments/assets/9c7f7478-febb-4527-999b-bbbf44af03ff


Perspective to create a 3d world. It's a line between our eyes and computer screen. */
/**  INTERVIEW QUESTIONS
/** ---------------------------------------- --> */

/*? 1: How can you use the translate transform function to move an element 50 pixels to the right and 20 pixels down? */
/* .element { transform: translate(50px, 20px); } */

/*? 2: Explain the scale transform function. How would you make an element twice its original size? */
/* .element { transform: scale(2); } */

/*? 3: How do you rotate an element 45 degrees clockwise using the rotate transform function? */
/* .element {  transform: rotate(45deg); } */

/*? 4: How can you combine multiple transform functions to perform complex transformations on an element? */
/* .element { transform: scale(1.5) rotate(45deg) translate(20px, 30px); } */

