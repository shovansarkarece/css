# CSS VARIABLES
### CSS variables, also known as CSS custom properties, allow you to define reusable values in your CSS code. They provide more flexibility and maintainability to your styles.
### 1)Declaration and Syntax:
- **Declare a CSS variable with the ```--``` prefix followed by a name. For example: ```--main-color.```**
- **Assign a value to the variable using the ```var()``` function, like this: ```var(--main-color)```.**
- **Variables can store various types of values, such as colors, numbers, text, and more.**
- **```--main-color: #3498db;```**

### 2) Variable Definition:
- **You can define variables in various places, including at the root level, within a selector, or even inside a specific CSS rule.**
- **```:root { --main-color: #3498db;  }```**
### 3)Variable Usage: 
- **Use the var keyword**
```
.button {
  ! background-color: var(--main-color);
} */
```
### Graphical-Example
![image](https://github.com/user-attachments/assets/64fbaf11-3d4f-4e33-a762-22e390220e03)
### Example
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Variables</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section class="hero-section">
      <div class="container">
        <div class="grid grid-two-column">
          <div class="hero-content">
            <h1>World Best CSS Course</h1>
            <p class="para-class" id="para-id">
              Unleash your web design potential with the best CSS course on the
              internet! 🚀 Elevate your skills, create stunning websites, and
              transform your career. Join us today and embark on a CSS journey
              like never before.
            </p>
            <a href="https://www.youtube.com/thapatechnical"> watch now </a>
          </div>
          <div class="hero-image">
            <figure>
              <img
                src="../images/hero.png"
                alt="headphone with black background"
              />
            </figure>
          </div>
        </div>
      </div>
    </section>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}
:root {
  --main-color: #0062ff;
  --supporting-color: #080a0c;
  --font-color: #fff;
  --bg-color: #080a0c;
  --btn-bg-color: #fff;
  --timepass-color: #fff;
}
body {
  background-color: var(--bg-color);
  color: var(--timepass-color);
  height: 100vh;
}
.container {
  height: 100vh;
  max-width: 1320px;
  padding: 64px 0;
  margin: 0 auto;
  display: grid;
  align-items: center;
}
.grid {
  display: grid;
  align-items: center;
  gap: 6.4rem;
}
.grid-two-column {
  grid-template-columns: repeat(2, 1fr);
}
.hero-content h1 {
  text-align: left;
  font-size: 54px;
  /* font-family: "Urbanist"; */
}
#para-id {
  color: pink;
}
.para-class {
  color: #0062ff;
}
p {
  font-size: 18px;
  letter-spacing: 1px;
  margin: 2rem 0 4rem 0;
  color: red;
}
img {
  width: 100%;
  height: auto;
}
.grid .hero-content a {
  background-color: var(--bg-color);
  border: 5px solid var(--timepass-color);
  display: inline-block;
  padding: 10px 32px;
  text-transform: capitalize;
  text-decoration: none;
  border-radius: 5px;
  font-size: 24px;
  font-weight: bold;
  -webkit-border-radius: 5px;
  -moz-border-radius: 5px;
  -ms-border-radius: 5px;
  -o-border-radius: 5px;
}
a {
  color: var(--timepass-color);
  background-color: red;
}
```
