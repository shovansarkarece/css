# Column_Layout
### The CSS multi-column layout allows easy definition of multiple columns of text - just like in newspapers */
- **column-count**
- **column-gap**
- **column-rule-style**
- **column-rule-width**
- **column-rule-color**
- **column-rule**
- **column-span**
- **column-width**

![image](https://github.com/user-attachments/assets/1d5c27ae-4be7-48e9-a840-c1fbb782d4ef)
### Example-1
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="color-style.css" />
    <title>color-in-css</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section class="hero-section">
      <br />
      <h1>Best CSS Course Ever Created</h1>
      <br />
      <p>
        Discover a world of possibilities with our comprehensive Thapa Technical
        CSS course. Dive into over 50 real-world interview questions to boost
        your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
        and tricks. Engage in dynamic learning with our animated PowerPoint
        presentations. Showcase your creativity with 10+ captivating animation
        projects. Take on the ultimate challenge with a mega, fully multipage
        responsive website project. Elevate your web presence with SEO insights
        and website performance testing. Plus, get expert guidance on choosing
        between free and paid hosting options. Our course is more than just CSS;
        it's your gateway to mastering web development.
      </p>
    </section>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: hsl(0, 0%, 94%);
  display: grid;
  place-items: center;
}

.hero-section {
  margin-top: 100px;
  width: 60%;
}

h1 {
  font-family: "Urbanist", sans-serif;
  font-size: 54px;
  font-weight: 900;
  /*? text properties starts here  */
  text-align: left;
  /* text-decoration-line: underline;
    -moz-text-decoration-line: underline; */
  text-decoration-style: double;
  -moz-text-decoration-style: double;
  text-decoration-color: #61677a;
  -moz-text-decoration-color: #61677a;
  text-decoration-thickness: 2px;
  text-transform: capitalize;
  letter-spacing: 2px;
  margin-bottom: 24px;
}

p {
  font-family: "Urbanist", sans-serif;
  font-size: 18px;
  font-weight: 400;
  /*? text properties starts here  */
  letter-spacing: 1px;
  word-spacing: 1px;
  line-height: 1.6;
  /* white-space: nowrap; all the text will be in one line  */
}

p {
  column-count: 3;
  column-rule: 4px solid red;
  /* column-rule-color: red;
  column-rule-style: dotted;
  column-rule-width: 10px; */
  column-gap: 50px;
  text-align: justify;
}
```
### Output
![image](https://github.com/user-attachments/assets/9a846c41-31a8-4371-950f-7bdffca57207)
