#  DISPLAY IN CSS  
![image](https://github.com/user-attachments/assets/0f56459d-4e5b-4330-aca9-f891d469e6aa)

- **Block-Level Elements:**
- **display: block 👉 The block value makes the element a block-level element. Block-level elements create a new "block formatting context" and take up the full width available.** 
- **They start on a new line,pushing subsequent elements below them.**
## New Line Start: 
- **They start on a new line in the webpage layout.**
## Full Width: 
- **They often take up the entire width of their container.**
### No Side-by-Side: 
- **They don't sit next to each other horizontally.**
- **Common Examples: Include paragraphs, headings, lists, and containers.**
- **Vertical Stacking: They stack on top of each other, creating a vertical layout.**
### Use Cases:
- **Creating standalone elements like paragraphs, headings, divs, and dividers.**
- **Structuring the main content of a webpage, such as articles or sections.** 
```
/*Block Level Elements*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Display-CSS</title>
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
      <h1 id="main-heading">CSS Display (Box Types)</h1>
      <div>
        <p>This is a block-level element.</p>
        <p>This is a block-level element.</p>
        <a href="#">Inline Level Element</a>
        <a href="#">Register Now</a>
        <!-- <br /> -->
        <a class="inline-block-elem" href="#">Inline Level Element</a>
        <a class="inline-block-elem" href="#">Register Now</a>
      </div>
    </section>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: Urbanist;
}
body {
  padding: 50px 100px;
  background-color: hsla(0, 0%, 94%);
}
#main-heading {
  color: #1e1403;
  text-align: left;
  font-size: 64px;
  margin-bottom: 30px;
}
p {
  width: 500px;
  margin: 0 auto;
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
  font-size: 24px;
  letter-spacing: 1.5px;
  background: linear-gradient(to right, #182848, #4b6cb7);
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  border-radius: 5px;
  color: #fff;
  -webkit-border-radius: 5px;
  -moz-border-radius: 5px;
  -ms-border-radius: 5px;
  -o-border-radius: 5px;
  padding: 30px 20px;
  margin-bottom: 24px;
}
a {
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
  font-size: 24px;
  letter-spacing: 1.5px;
  background: linear-gradient(to right, #182848, #4b6cb7);
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  color: #fff;
  border-radius: 5px;
  /* width: 500px; */
  /* height: 100px; */
  padding: 15px 36px;
  border: 1px solid red;
  margin-top: 100px;
  margin-right: 30px;
  /* display: inline-block; */
  display: block;
  /* display: inline; */
}
/* this is just to for styling th background */
p:nth-of-type(2),
a:nth-of-type(2),
.inline-block-elem:last-child {
  background: linear-gradient(to right, #514a9d, #24c6dc);
  display: none;
}
```
### Output 
![image](https://github.com/user-attachments/assets/ca2aeb1e-f05a-4c14-b2b4-b041e891f4a6)

### Inline Elements 
### display: inline  
- **👉 The inline value makes the element an inline-level element. Inline elements only take up as much width as necessary, and they do not create a new block formatting context. Inline elements can appear on the same line as other inline elements.**
- **display: inline; elements don't respect top and bottom margins or padding, only left and right. Also width and height is not accepted.**
- **Inline Flow: They flow within the content and don't start on new lines.**
- **Space-Efficient: They take up only as much width as necessary.**
- **Side-by-Side: They can sit next to each other horizontally.**
- **Common Examples: Include links, spans, and emphasis tags.**
- **Text Enhancements: Often used for styling text or adding small inline elements.**
### Use Cases:
- **Styling text elements like links (<a>) or spans within paragraphs.**
- **Displaying elements side by side within a paragraph.**
```
/*Block Level Elements*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Display-CSS</title>
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
      <h1 id="main-heading">CSS Display (Box Types)</h1>
      <div>
        <p>This is a block-level element.</p>
        <p>This is a block-level element.</p>
        <a href="#">Inline Level Element</a>
        <a href="#">Register Now</a>
        <!-- <br /> -->
        <a class="inline-block-elem" href="#">Inline Level Element</a>
        <a class="inline-block-elem" href="#">Register Now</a>
      </div>
    </section>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: Urbanist;
}
body {
  padding: 50px 100px;
  background-color: hsla(0, 0%, 94%);
}
#main-heading {
  color: #1e1403;
  text-align: left;
  font-size: 64px;
  margin-bottom: 30px;
}
p {
  width: 500px;
  margin: 0 auto;
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
  font-size: 24px;
  letter-spacing: 1.5px;
  background: linear-gradient(to right, #182848, #4b6cb7);
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  border-radius: 5px;
  color: #fff;
  -webkit-border-radius: 5px;
  -moz-border-radius: 5px;
  -ms-border-radius: 5px;
  -o-border-radius: 5px;
  padding: 30px 20px;
  margin-bottom: 24px;
}
a {
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
  font-size: 24px;
  letter-spacing: 1.5px;
  background: linear-gradient(to right, #182848, #4b6cb7);
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  color: #fff;
  border-radius: 5px;
  /* width: 500px; */
  /* height: 100px; */
  padding: 15px 36px;
  border: 1px solid red;
  margin-top: 100px;
  margin-right: 30px;
  /* display: inline-block; */
  /* display: block;*/
  display: inline; 
}
/* this is just to for styling th background */
p:nth-of-type(2),
a:nth-of-type(2),
.inline-block-elem:last-child {
  background: linear-gradient(to right, #514a9d, #24c6dc);
  display: none;
}
```
### Output
![image](https://github.com/user-attachments/assets/a056279c-fd83-4cb0-842b-bf74956098d6)

### Inline-Block Elements:
- **display: inline-block 👉  The inline-block value combines aspects of both block and inline. Elements with inline-block behave like inline elements but can have dimensions (width and height) and vertical alignment.**
- **Mixed Behavior: They combine aspects of both inline and block elements.**
- **Width and Height: You can set their dimensions (width and height).**
- **In-Line Flow: They can sit next to each other horizontally.**
- **Space-Efficient: They take up only as much width as necessary.**
- **Common Examples: Used for creating custom-styled buttons, images with captions,**
### Use Cases:
- **Creating custom-styled buttons.**
- **Displaying images with captions or descriptions next to them.**
```
/*Block Level Elements*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Display-CSS</title>
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
      <h1 id="main-heading">CSS Display (Box Types)</h1>
      <div>
        <p>This is a block-level element.</p>
        <p>This is a block-level element.</p>
        <a href="#">Inline Level Element</a>
        <a href="#">Register Now</a>
        <!-- <br /> -->
        <a class="inline-block-elem" href="#">Inline Level Element</a>
        <a class="inline-block-elem" href="#">Register Now</a>
      </div>
    </section>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  font-family: Urbanist;
}
body {
  padding: 50px 100px;
  background-color: hsla(0, 0%, 94%);
}
#main-heading {
  color: #1e1403;
  text-align: left;
  font-size: 64px;
  margin-bottom: 30px;
}
p {
  width: 500px;
  margin: 0 auto;
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
  font-size: 24px;
  letter-spacing: 1.5px;
  background: linear-gradient(to right, #182848, #4b6cb7);
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  border-radius: 5px;
  color: #fff;
  -webkit-border-radius: 5px;
  -moz-border-radius: 5px;
  -ms-border-radius: 5px;
  -o-border-radius: 5px;
  padding: 30px 20px;
  margin-bottom: 24px;
}
a {
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
  font-size: 24px;
  letter-spacing: 1.5px;
  background: linear-gradient(to right, #182848, #4b6cb7);
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  color: #fff;
  border-radius: 5px;
  /* width: 500px; */
  /* height: 100px; */
  padding: 15px 36px;
  border: 1px solid red;
  margin-top: 100px;
  margin-right: 30px;
   display: inline-block; 
}
/* this is just to for styling th background */
p:nth-of-type(2),
a:nth-of-type(2),
.inline-block-elem:last-child {
  background: linear-gradient(to right, #514a9d, #24c6dc);
  display: none;
}
```
### Output 
![image](https://github.com/user-attachments/assets/a056279c-fd83-4cb0-842b-bf74956098d6)
# Interview Question
- **1: What does display: none; do to an element's accessibility?**
- **It makes the element completely inaccessible to screen readers and keyboard navigation.**

- **2: How do you center an element horizontally using display: block;?**
- **To center a display: block; element horizontally, you can set its left and right margins to auto.**

- **4: What is the default behavior of display: inline; elements with regard to margin and padding?**
- **display: inline; elements don't respect top and bottom margins or padding, only left and right. Also width and height is not accepted.*

- **5: How can you make an inline element like a link or a span act like a block-level element? ⭐⭐**
- **You can apply display: block; or display: inline-block; to make an inline element behave like a block-level element.**

/*? 6: What is the impact of applying display: block; to an anchor <a> element? */
/* Applying display: block; to an anchor element allows you to set its width, height, and apply padding or margin. This is often used for creating custom-styled buttons. */
