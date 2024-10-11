# OVERFLOW IN CSS
![image](https://github.com/user-attachments/assets/4350f1a3-adbd-4bee-9538-b3942272d23f)
# Example of Overflow
![image](https://github.com/user-attachments/assets/3ab316b8-2407-4c8a-a167-d3f97010ea26)
- **The overflow property in CSS is used to control how content overflows its containing element when it doesn't fit within the available space. It's a useful property for handling content that exceeds its container's dimensions.**
# Overflow:scroll
- **Scrollbars (both horizontal and vertical) are added to the container, allowing users to scroll to see the hidden content.**
- **Use it when you want to display all content and provide a scrolling mechanism.**
### Example
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1 id="main-heading">CSS Overflow</h1>
    <hr />
    <br />
    <section>
      <div class="overflow-div">
        <p>
          Discover a world of possibilities with Thapa Technical comprehensive
          CSS course. Dive into over 50 real-world interview questions to boost
          your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
          and tricks. Engage in dynamic learning with our animated PowerPoint
          presentations. Showcase your creativity with 10+ captivating animation
          projects. Take on the ultimate challenge with a mega, fully multipage
          responsive website project. Elevate your web presence with SEO
          insights and website performance testing. Plus, get expert guidance on
          choosing between free and paid hosting options. Our course is more
          than just CSS; it's your gateway to mastering web development.
        </p>
      </div>
      <br />
      <!-- <div class="overflow-div-2">
        <p>
          Discover a world of possibilities with Thapa Technical comprehensive
          CSS course. Dive into over 50 real-world interview questions to boost
          your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
          and tricks. Engage in dynamic learning with our animated PowerPoint
          presentations. Showcase your creativity with 10+ captivating animation
          projects. Take on the ultimate challenge with a mega, fully multipage
          responsive website project. Elevate your web presence with SEO
          insights and website performance testing. Plus, get expert guidance on
          choosing between free and paid hosting options. Our course is more
          than just CSS; it's your gateway to mastering web development.
        </p>
      </div> -->
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
}
#main-heading {
  font-size: 6.2rem;
  color: #1e1403;
  margin: 3rem 0;
}
p {
  line-height: 40px;
  font-size: 2rem;
}
.overflow-div {
  width: 600px;
  height: 300px;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 6px 24px 0px,
    rgba(0, 0, 0, 0.08) 0px 0px 0px 1px;
  border: 5px solid #9eb384;
  padding: 10px;
  /* our code will start from here  */
  /* overflow-y: scroll; */
  /* overflow-x: scroll; */
   overflow: scroll; 
}
.overflow-div-2 {
  width: 600px;
  height: 300px;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 6px 24px 0px,
    rgba(0, 0, 0, 0.08) 0px 0px 0px 1px;
  border: 5px solid #9eb384;
  padding: 10px;
}
```
### Output
![image](https://github.com/user-attachments/assets/ea469e5a-4128-42b2-a0f0-506a313bcfcf)
# Overflow: Visible (Default)
- **This is the default behavior where content can overflow its container without any clipping. Use it when you want content to extend beyond its container's boundaries.**
### Example
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1 id="main-heading">CSS Overflow</h1>
    <hr />
    <br />
    <section>
      <div class="overflow-div">
        <p>
          Discover a world of possibilities with Thapa Technical comprehensive
          CSS course. Dive into over 50 real-world interview questions to boost
          your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
          and tricks. Engage in dynamic learning with our animated PowerPoint
          presentations. Showcase your creativity with 10+ captivating animation
          projects. Take on the ultimate challenge with a mega, fully multipage
          responsive website project. Elevate your web presence with SEO
          insights and website performance testing. Plus, get expert guidance on
          choosing between free and paid hosting options. Our course is more
          than just CSS; it's your gateway to mastering web development.
        </p>
      </div>
      <br />
      <!-- <div class="overflow-div-2">
        <p>
          Discover a world of possibilities with Thapa Technical comprehensive
          CSS course. Dive into over 50 real-world interview questions to boost
          your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
          and tricks. Engage in dynamic learning with our animated PowerPoint
          presentations. Showcase your creativity with 10+ captivating animation
          projects. Take on the ultimate challenge with a mega, fully multipage
          responsive website project. Elevate your web presence with SEO
          insights and website performance testing. Plus, get expert guidance on
          choosing between free and paid hosting options. Our course is more
          than just CSS; it's your gateway to mastering web development.
        </p>
      </div> -->
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
}
#main-heading {
  font-size: 6.2rem;
  color: #1e1403;
  margin: 3rem 0;
}
p {
  line-height: 40px;
  font-size: 2rem;
}
.overflow-div {
  width: 600px;
  height: 300px;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 6px 24px 0px,
    rgba(0, 0, 0, 0.08) 0px 0px 0px 1px;
  border: 5px solid #9eb384;
  padding: 10px;
  /* our code will start from here  */
   overflow: visible;
  /* overflow: hidden; */
  /* overflow-y: scroll; */
  /* overflow-x: scroll; */
  /* overflow: scroll; */
  /* white-space: nowrap; */
  /* overflow: auto; */
}
.overflow-div-2 {
  width: 600px;
  height: 300px;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 6px 24px 0px,
    rgba(0, 0, 0, 0.08) 0px 0px 0px 1px;
  border: 5px solid #9eb384;
  padding: 10px;
}
```
### Output
![image](https://github.com/user-attachments/assets/17d95377-88fa-48d3-a624-7e448a2776e6)
# Overflow: Hidden
- **Content that overflows the container is hidden and not visible.**
- **Useful when you want to hide extra content that doesn't fit within a fixed-size container.**
### Example
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1 id="main-heading">CSS Overflow</h1>
    <hr />
    <br />
    <section>
      <div class="overflow-div">
        <p>
          Discover a world of possibilities with Thapa Technical comprehensive
          CSS course. Dive into over 50 real-world interview questions to boost
          your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
          and tricks. Engage in dynamic learning with our animated PowerPoint
          presentations. Showcase your creativity with 10+ captivating animation
          projects. Take on the ultimate challenge with a mega, fully multipage
          responsive website project. Elevate your web presence with SEO
          insights and website performance testing. Plus, get expert guidance on
          choosing between free and paid hosting options. Our course is more
          than just CSS; it's your gateway to mastering web development.
        </p>
      </div>
      <br />
      <!-- <div class="overflow-div-2">
        <p>
          Discover a world of possibilities with Thapa Technical comprehensive
          CSS course. Dive into over 50 real-world interview questions to boost
          your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
          and tricks. Engage in dynamic learning with our animated PowerPoint
          presentations. Showcase your creativity with 10+ captivating animation
          projects. Take on the ultimate challenge with a mega, fully multipage
          responsive website project. Elevate your web presence with SEO
          insights and website performance testing. Plus, get expert guidance on
          choosing between free and paid hosting options. Our course is more
          than just CSS; it's your gateway to mastering web development.
        </p>
      </div> -->
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
}
#main-heading {
  font-size: 6.2rem;
  color: #1e1403;
  margin: 3rem 0;
}
p {
  line-height: 40px;
  font-size: 2rem;
}
.overflow-div {
  width: 600px;
  height: 300px;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 6px 24px 0px,
    rgba(0, 0, 0, 0.08) 0px 0px 0px 1px;
  border: 5px solid #9eb384;
  padding: 10px;
  /* our code will start from here  */
   overflow: auto; 
}
.overflow-div-2 {
  width: 600px;
  height: 300px;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 6px 24px 0px,
    rgba(0, 0, 0, 0.08) 0px 0px 0px 1px;
  border: 5px solid #9eb384;
  padding: 10px;
}
```
### Output
![image](https://github.com/user-attachments/assets/21e717ee-815c-4e65-96c0-70605fbc8ff9)
# Overflow: Auto
- **Scrollbars are added only when content overflows the container.**
- **It's a combination of visible (no scrollbars if content fits) and scroll (scrollbars when content overflows). Ideal for creating scrollable containers only when needed.**
### Example
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1 id="main-heading">CSS Overflow</h1>
    <hr />
    <br />
    <section>
      <div class="overflow-div">
        <p>
          Discover a world of possibilities with Thapa Technical comprehensive
          CSS course. Dive into over 50 real-world interview questions to boost
          your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
          and tricks. Engage in dynamic learning with our animated PowerPoint
          presentations. Showcase your creativity with 10+ captivating animation
          projects. Take on the ultimate challenge with a mega, fully multipage
          responsive website project. Elevate your web presence with SEO
          insights and website performance testing. Plus, get expert guidance on
          choosing between free and paid hosting options. Our course is more
          than just CSS; it's your gateway to mastering web development.
        </p>
      </div>
      <br />
      <!-- <div class="overflow-div-2">
        <p>
          Discover a world of possibilities with Thapa Technical comprehensive
          CSS course. Dive into over 50 real-world interview questions to boost
          your job prospects. Unlock the secrets of CSS with 30+ invaluable tips
          and tricks. Engage in dynamic learning with our animated PowerPoint
          presentations. Showcase your creativity with 10+ captivating animation
          projects. Take on the ultimate challenge with a mega, fully multipage
          responsive website project. Elevate your web presence with SEO
          insights and website performance testing. Plus, get expert guidance on
          choosing between free and paid hosting options. Our course is more
          than just CSS; it's your gateway to mastering web development.
        </p>
      </div> -->
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
}
#main-heading {
  font-size: 6.2rem;
  color: #1e1403;
  margin: 3rem 0;
}
p {
  line-height: 40px;
  font-size: 2rem;
}
.overflow-div {
  width: 600px;
  height: 300px;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 6px 24px 0px,
    rgba(0, 0, 0, 0.08) 0px 0px 0px 1px;
  border: 5px solid #9eb384;
  padding: 10px;
  /* our code will start from here  */
   overflow: hidden; 
}
.overflow-div-2 {
  width: 600px;
  height: 300px;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 6px 24px 0px,
    rgba(0, 0, 0, 0.08) 0px 0px 0px 1px;
  border: 5px solid #9eb384;
  padding: 10px;
}
```
### Output
![image](https://github.com/user-attachments/assets/0ea0c698-d897-43f8-8c86-2ee5f2f78097)
# INTERVIEW QUESTIONS
- **1: How does the overflow: hidden; property value work?**
- **When overflow is set to hidden, any content that overflows the container's box is clipped and not visible. It effectively hides the overflowed content.**
- **2: What is the difference between overflow: auto; and overflow: scroll;?**
- **Both overflow: auto; and overflow: scroll; display scrollbars when content overflows. However, overflow: auto; only shows scrollbars when content overflows, while overflow: scroll; always displays scrollbars.**
- **3: How can you make an element scrollable only horizontally (horizontally overflowed content) while hiding the vertical overflow?**
- **You can achieve this by setting overflow-x: auto; to allow horizontal scrolling and overflow-y: hidden; to hide vertical overflow. Also, we use overflow-x: scroll; white-space: nowrap**
