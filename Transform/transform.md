# Transition
![image](https://github.com/user-attachments/assets/32cfd6c3-4fc1-46a6-9456-1e07f0a8578a)

# 1)transition-property: Specifies which CSS properties should be transitioned.
- **Example: Transitioning the color and background-color properties.**
#### Syntax
```
.element {
  transition-property: color, background-color;
} 
```
# 2)transition-duration: Defines how long the transition should take to complete.
- **Transitioning over 1 second.**
#### Syntax
```
.element {
  transition-duration: 1s;
} */
```
- **It accept s and ms values too Transition options**

# 3)transition-timing-function: Specifies the timing curve used for the transition.
- **Example: Using ease-in-out for a smooth start and end.**
#### Syntax
```
.element {
  transition-timing-function: ease;/ease-in-out;/ease-in;/
} */
```
# 4)transition-delay: Sets a delay before the transition starts.
- **Example: Starting the transition after 0.5 seconds.**
#### Syntax
```
.element {
  transition-delay: 2s;
} */
```
# shorthand property of all 4 is simply to write transition */
- **property name | duration | easing function | delay**
- **transition: margin-right 4s ease-in-out 1s;**
### Example of Transition and it's shortend
#### Syntax of shortend of transition and transition property
```
/*  property name | duration | easing function | delay */
   transition-property: width, color, background-color; 
   transition-duration: 1s;
  transition-timing-function: linear;
  transition-delay: 2s;
/*shortened*/
transition: all 1s linear 2s;
```
#### Example
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Transition in CSS</title>
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
            <h1>Best CSS Course Ever</h1>
            <p>
              Unleash your web design potential with the best CSS course on the
              internet! 🚀 Elevate your skills, create stunning websites, and
              transform your career. Join us today and embark on a CSS journey
              like never before.
            </p>
            <a href="https://www.youtube.com/thapatechnical"> Listen Now </a>
          </div>
          <div class="hero-image">
            <figure>
              <img src="../../images/css.png" alt="thapa technical " />
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
body {
  background-color: #080a0c;
  color: azure;
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
  gap: 64px;
}
.grid-two-column {
  grid-template-columns: repeat(2, 1fr);
}
.hero-content h1 {
  font-size: 48px;
  text-align: left;
}
.hero-content p {
  font-size: 18px;
  letter-spacing: 1px;
  margin: 20px 0 40px 0;
}
img {
  max-width: 80%;
  height: auto;
}

a {
  background-color: transparent;
  display: inline-block;
  padding: 12px 32px;
  text-decoration: none;
  border-radius: 05px;
  font-size: 24px;
  font-weight: bold;
  border: 5px solid #fff;
  color: #fff;
  width: 200px;
  text-align: center;
  /*?TRANSITIONCODESTARTSHERE*/
  /* transition-property: width, color, background-color; */
  /* transition-duration: 1s;
  transition-timing-function: linear;
  transition-delay: 2s; */
  transition: all 1s linear;
}
.hero-content a:hover {
  background-color: blue;
  color: #fff;
  width: 400px;
  box-shadow: rgba(255, 255, 255, 0.8) 0px 19px 38px,
    rgba(255, 255, 255, 0.5) 0px 15px 12px;
}

img {
  transition: scale 1s linear;
}
img:hover {
  scale: 1.2;
}

```

### Output
https://github.com/user-attachments/assets/fd2ac2c8-44db-4e19-bb7d-00f4b1ce048a

