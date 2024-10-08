# BOX SHADOW
- **CSS3 Box Shadow is a new property to add shadow effects to any html Element. You can choose your own  offset, blur, color, spread/density and repetition. Unlike border, it not a part of CSS Box Model, thus 
doesn't effect the layout even if it is bigger in size. Also we can add multiple shadows with different colors and offsets.**
- **Outer Box Shadow: Default box shadow is outer. x-offset and y-offset are compulsory properties, rest all are optional.**
- **Inner Box Shadow: To use inner box shadow, use inset. Inset is only required if shadow is inside. By-default shadow is outside.**
![image](https://github.com/user-attachments/assets/dc0c58cd-0317-40be-944e-276106a6c0a9)
## Example-1
```
//////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Box-Shadow in CSS</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <div class="shadow"></div>
    </section>
  </body>
</html>
//////Style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-color: #191717;
  display: grid;
  place-items: center;
}
.shadow {
  width: 300px;
  height: 300px;
  padding: 40px;
  background-color: rgb(174, 68, 90);
  border-radius: 50%;
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  -ms-border-radius: 50%;
  -o-border-radius: 50%;
  /*? box shadow here  */
  box-shadow: 0 0 0 60px #ffb000;////-->4th parameter is for density
}
```
## Output
![image](https://github.com/user-attachments/assets/d7278090-1b3d-487f-9f5f-7f78e3d79800)
## Example-2( Offset-X)
```
//////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Box-Shadow in CSS</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <div class="shadow"></div>
    </section>
  </body>
</html>
//////Style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-color: #191717;
  display: grid;
  place-items: center;
}
.shadow {
  width: 300px;
  height: 300px;
  padding: 40px;
  background-color: rgb(174, 68, 90);
  border-radius: 50%;
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  -ms-border-radius: 50%;
  -o-border-radius: 50%;
  /*? box shadow here  */
  box-shadow: 20px 0px 0 60px #ffb000;////-->1st parameter is for Offset-X  means horizontally it will shift
}
```
## Output
![image](https://github.com/user-attachments/assets/56e71359-4003-488c-bf62-dd1b7a7700c0)
## Example-3( Offset-Y)
```
//////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Box-Shadow in CSS</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <div class="shadow"></div>
    </section>
  </body>
</html>
//////Style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-color: #191717;
  display: grid;
  place-items: center;
}
.shadow {
  width: 300px;
  height: 300px;
  padding: 40px;
  background-color: rgb(174, 68, 90);
  border-radius: 50%;
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
  -ms-border-radius: 50%;
  -o-border-radius: 50%;
  /*? box shadow here  */
  box-shadow: 20px 0px 0 60px #ffb000;////-->1st parameter is for Offset-X  means horizontally it will shift
}
```
box-shadow: 0px 40px 0 60px #ffb000;
## Output
![image](https://github.com/user-attachments/assets/b5226398-3d31-40ad-bcc5-064b4ea3feb6)

# Disclaimer
- **In most the cases we are using below link**
- 1)[box-shadow](https://getcssscan.com/css-box-shadow-examples)
