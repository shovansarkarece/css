# FILTERS

- **CSS filters are a set of graphical effects that can be applied to HTML elements to modify their appearance. Filters can alter properties like color, brightness, contrast, and more.**
- **CSS filters can be combined by separating them with spaces.**
- **Filters can be applied to images, backgrounds, and even entire sections of a webpage.**
- **Experiment with filter values to create unique visual effects.**
- **Be cautious with excessive use of filters, as they can significantly alter the appearance of elements.**

## Commonly Used Filter Functions
- **(i)grayscale()**
- **(ii)blur()**
- **(iii)brightness()**
- **(iv)contrast()**
- **(v)saturate()**
- **(vi)hue-rotate()**
- **(vii)invert()**
- **(viii)opacity()**

## grayscale(): Converts the element to grayscale. A value of 1 (or 100%) means fully grayscale.
- **```filter: grayscale(0.5);``` --> It means 50% grayscale** 
### Example-1
```
/////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Filters In CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../images/html.png" alt="thapa techncial html course" />
    </section>
  </body>
</html>
/////style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
section {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}
img {
  width: 50%;
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  -ms-border-radius: 20px;
  -o-border-radius: 20px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
    rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
  filter: grayscale(0.5);
}
```
## Output
![image](https://github.com/user-attachments/assets/311a3b30-7463-4090-8ff6-d77535596aff)
## blur(): Applies a blur effect to the element. The value determines the amount of blur.
- **```filter: blur(5px)```--> It means 5 pixels of blur.**
### Example-2
```
/////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Filters In CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../images/html.png" alt="thapa techncial html course" />
    </section>
  </body>
</html>
/////style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
section {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}
img {
  width: 50%;
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  -ms-border-radius: 20px;
  -o-border-radius: 20px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
    rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
  filter: blur(5px);
}
```
## Output
![image](https://github.com/user-attachments/assets/a690c4d6-bbb9-4695-91e9-e40bd7df5664)
## brightness(): Adjusts the brightness of the element. Values greater than 1 increase brightness, and values less than 1 decrease it. */
- **```filter: brightness(1.5);``` -->It means 150% brightness.**
### Example-3
```
/////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Filters In CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../images/html.png" alt="thapa techncial html course" />
    </section>
  </body>
</html>
/////style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
section {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}
img {
  width: 50%;
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  -ms-border-radius: 20px;
  -o-border-radius: 20px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
    rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
   filter: brightness(150%);   /* filter: brightness(1.5);*/ /*It means 150% brightness.*/
}
```
## Output
![image](https://github.com/user-attachments/assets/e9d5fa3d-dab2-49ad-9afe-9e9a500772cb)
## contrast(): Adjusts the contrast of the element. Similar to brightness(), values greater than 1 increase contrast, and values less than 1 decrease it.
- **```filter: contrast(0.8);```-->It means 80% contrast.**
### Example-4
```
/////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Filters In CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../images/html.png" alt="thapa techncial html course" />
    </section>
  </body>
</html>
/////style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
section {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}
img {
  width: 50%;
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  -ms-border-radius: 20px;
  -o-border-radius: 20px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
    rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
   contrast(150%); /*150% contrast*/
}
```
## Output
![image](https://github.com/user-attachments/assets/828d953b-cb8f-485c-bf67-eb56708ef0a4)
## saturate(): Increases or decreases the saturation of the element. Values greater than 1 increase saturation, and values less than 1 desaturate it.
- **```filter: saturate(2);```-->It means Double saturation**
### Example-5
```
/////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Filters In CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../images/html.png" alt="thapa techncial html course" />
    </section>
  </body>
</html>
/////style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
section {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}
img {
  width: 50%;
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  -ms-border-radius: 20px;
  -o-border-radius: 20px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
    rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
    filter: saturate(5);/**/
}
```
### Output
![image](https://github.com/user-attachments/assets/19038da9-52af-4553-8f02-d64983a62703)
## hue-rotate(): Rotates the hues of the element. Values are in degrees. */
- **```filter: hue-rotate(90deg);```--> It means 90-degree hue rotation.**
### Example-6
```
/////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Filters In CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../images/html.png" alt="thapa techncial html course" />
    </section>
  </body>
</html>
/////style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
section {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}
img {
  width: 50%;
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  -ms-border-radius: 20px;
  -o-border-radius: 20px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
    rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
    filter: saturate(5);/**/
}
```
### Output
![image](https://github.com/user-attachments/assets/3920c191-880d-4b9d-a76e-0d85cf047a54)

## invert(): Inverts the colors of the element. A value of 1 (or 100%) inverts completely. */
- **```filter: invert(0.7);```--> 70% color inversion**
### Example-7
```
/////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Filters In CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../images/html.png" alt="thapa techncial html course" />
    </section>
  </body>
</html>
/////style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
section {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}
img {
  width: 50%;
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  -ms-border-radius: 20px;
  -o-border-radius: 20px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
    rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
     filter: invert(0.7); /*70% color inversion*/
}
```

### Output
![image](https://github.com/user-attachments/assets/f975a8ea-6fd5-4612-9ae6-12521108df45)


/*? opacity(): Adjusts the opacity (transparency) of the element. Values range from 0 (completely transparent) to 1 (completely opaque). */
/* filter: opacity(0.5); 50% opacity */

### Example-7
```
/////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Filters In CSS</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../images/html.png" alt="thapa techncial html course" />
    </section>
  </body>
</html>
/////style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: "Urbanist";
}
section {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}
img {
  width: 50%;
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  -ms-border-radius: 20px;
  -o-border-radius: 20px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 10px 36px 0px,
    rgba(0, 0, 0, 0.06) 0px 0px 0px 1px;
      filter: opacity(0.5); /*50% opacity */
}
```

### Output
![image](https://github.com/user-attachments/assets/b50b7056-2d54-4bae-b81d-c3e252695554)
# INTERVIEW QUESTIONS
## 1: What are CSS filters, and why are they used? */
- **CSS filters are visual effects applied to HTML elements to modify their appearance. They are used to change properties like color, brightness, contrast, etc., without altering the underlying content.**
## 2: How can you create a blur effect on an element using CSS filters? */
- **The blur() filter function is used for blurring. You can specify the blur amount in pixels, like filter: blur(5px);.**
## 3: How can you combine multiple filters to create complex effects? */
- **You can apply multiple filter functions to an element, separating them with spaces. For example: filter: blur(3px) grayscale(0.5) contrast(1.2).like using this code ```filter: blur(3px) grayscale(0.5) contrast(1.2);```**
