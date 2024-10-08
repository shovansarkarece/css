# FILTERS

- **CSS filters are a set of graphical effects that can be applied to HTML elements to modify their appearance. Filters can alter properties like color, brightness, contrast, and more.**

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
```
## Output
![image](https://github.com/user-attachments/assets/311a3b30-7463-4090-8ff6-d77535596aff)
## blur(): Applies a blur effect to the element. The value determines the amount of blur.

/* filter: blur(5px); 5 pixels of blur */

/*? brightness(): Adjusts the brightness of the element. Values greater than 1 increase brightness, and values less than 1 decrease it. */
/* filter: brightness(1.5); 150% brightness */

/*? contrast(): Adjusts the contrast of the element. Similar to brightness(), values greater than 1 increase contrast, and values less than 1 decrease it. */
/* filter: contrast(0.8); 80% contrast */

/*? saturate(): Increases or decreases the saturation of the element. Values greater than 1 increase saturation, and values less than 1 desaturate it. */
/* filter: saturate(2); Double saturation */

/*? hue-rotate(): Rotates the hues of the element. Values are in degrees. */
/* filter: hue-rotate(90deg); 90-degree hue rotation */

/*? invert(): Inverts the colors of the element. A value of 1 (or 100%) inverts completely. */
/* filter: invert(0.7); 70% color inversion */

/*? opacity(): Adjusts the opacity (transparency) of the element. Values range from 0 (completely transparent) to 1 (completely opaque). */
/* filter: opacity(0.5); 50% opacity */

/*? sepia(): Applies a sepia tone effect to the element. A value of 1 (or 100%) is full sepia. */
/* filter: sepia(0.7); 70% sepia effect */

/** ------------------------------------- -->
/** IMPORTANT TIPS - FILTERS - CSS3
/** ---------------------------------------- --> */

/* CSS filters can be combined by separating them with spaces.
Filters can be applied to images, backgrounds, and even entire sections of a webpage.
Experiment with filter values to create unique visual effects.
Be cautious with excessive use of filters, as they can significantly alter the appearance of elements. */
