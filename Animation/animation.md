# Animation
## animation-name: This property specifies the name of the keyframe animation you want to apply to an element.
- **Example: animation-name: myAnimation;**

## animation-duration: Sets the duration of the animation in seconds (s) or milliseconds (ms).
- **Example: animation-duration: 2s;**

## animation-timing-function: Defines the timing function that determines the acceleration and deceleration of the animation.
- **Common values include ease, linear, ease-in, ease-out, ease-in-out, and more.**
- **Example: animation-timing-function: ease-in-out;**

## animation-delay: Specifies a delay before the animation starts. It can be in seconds (s) or milliseconds (ms).
- **Example: animation-delay: 1s;**

## animation-iteration-count: Sets the number of times the animation should repeat. You can use values like infinite, 3, or 2n (for even iterations).
- **Example: animation-iteration-count: infinite;**

## animation-direction: Determines whether the animation runs forwards, backward, or alternates between forward and backward cycles.
- **Values include normal, reverse, alternate, and alternate-reverse.**
- **Example: animation-direction: alternate;**

# Very Very Important 
- **@keyframes:**
- **This is not a property but a rule used to define the animation's keyframes. Keyframes specify how the element should look at various points during the animation.**
### Example-1
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Animation in CSS</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <h1>CSS Animation</h1>
      <div class="box"></div>
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
  background-color: #2b3033;
}
.container {
  width: 100vw;
  height: 100vh;
}
h1 {
  padding: 50px;
  color: #fff;
  font-size: 48px;
}
.box {
  width: 100px;
  height: 100px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 50px;
  display: inline-block;
  border-radius: 50%;
  /*? animation start here  */
  /* -------------------------------------Example of animation lefttoright------------------------------------------ */
  animation-name: lefttoright;
  animation-duration: 3s;
  animation-timing-function: linear;
  animation-iteration-count: 2; 
  animation-direction: normal;
}
@keyframes lefttoright {
  from {
    translate: 0%;
  }
  to {
translate: 90vw;
/* translate: calc(90vw - 100px); */
  }
} 
```
### Output
https://github.com/user-attachments/assets/f89301f0-fae0-4f7e-aea7-bfa7aa5d7b71
### Example-2
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Animation in CSS</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <h1>CSS Animation</h1>
      <div class="box"></div>
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
  background-color: #2b3033;
}
.container {
  width: 100vw;
  height: 100vh;
}
h1 {
  padding: 50px;
  color: #fff;
  font-size: 48px;
}
.box {
  width: 100px;
  height: 100px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 50px;
  display: inline-block;
  border-radius: 50%;
  /*? animation start here  */
  /* -------------------------------------Example of animation lefttoright------------------------------------------ */
  animation-name: lefttoright;
  animation-duration: 3s;
  animation-timing-function: linear;
  animation-iteration-count: 2; 
  animation-direction: alternate;
}
@keyframes lefttoright {
  from {
    translate: 0%;
  }
  to {
translate: 90vw;
/* translate: calc(90vw - 100px); */
  }
} 
```
### Output
https://github.com/user-attachments/assets/95826362-266a-442d-ba3c-6434a3db1238
### Example-3
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Animation in CSS</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <h1>CSS Animation</h1>
      <div class="box"></div>
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
  background-color: #2b3033;
}
.container {
  width: 100vw;
  height: 100vh;
}
h1 {
  padding: 50px;
  color: #fff;
  font-size: 48px;
}
.box {
  width: 100px;
  height: 100px;
  background-color: #4861ec;
  box-shadow: 0 0 0px 15px #353f6d;
  margin: 50px;
  display: inline-block;
  border-radius: 50%;
  /*? animation start here  */
  /* -------------------------------------Example of animation lefttoright------------------------------------------ */
  animation-name: lefttoright;
  animation-duration: 3s;
  animation-timing-function: linear;
  animation-iteration-count: 2; 
  animation-direction: alternate-reverse;
}
@keyframes lefttoright {
  from {
    translate: 0%;
  }
  to {
translate: 90vw;
/* translate: calc(90vw - 100px); */
  }
} 
```
### Output

https://github.com/user-attachments/assets/684db0bd-653a-4c39-aee0-147446192fc4


