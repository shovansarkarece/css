# Position
![image](https://github.com/user-attachments/assets/5098c9eb-e23c-42b4-b9e9-518e5ce4f3f9)
- **The position property in CSS is used to control the positioning of elements within a web page.**
- **It defines how an element should be placed relative to its normal position in the document flow or relative to its parent or containing elements.**
### Position: relative; 
-- **If we want to move our child dev anywhere then keep that child div into parent div and always parent must be relative and child must be absolute.**
![image](https://github.com/user-attachments/assets/6d40f415-f357-47de-8b07-5a2b55579462)
## Some example of ```parent's position:relative chil'd position:absolute``
### Example-1
![image](https://github.com/user-attachments/assets/8d7ade6a-291b-4965-a78a-24bce2d62179)
### Example-2
![image](https://github.com/user-attachments/assets/b7d6a51e-00e2-43ad-bb45-2ee4297553a6)
### Example-3
![image](https://github.com/user-attachments/assets/d0616a88-1a74-4c31-adf5-0cd665c6350a)
### Example-4
![image](https://github.com/user-attachments/assets/d54117e2-e3c3-4e6b-a298-8f8ebb027eaf)
### Example-5
![image](https://github.com/user-attachments/assets/73f39ae2-fc62-4370-b515-4e173c3601c7)
### Example-6
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Position Absolute</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1 id="main-heading">CSS Positions</h1>
    <section class="parent-div">
      <div class="child child-1">child 1</div>
      <div class="child child-2">child 2</div>
      <div class="child child-3">child 3</div>
      <div class="child child-4">child 4</div>
      <div class="child child-5">child 5</div>
    </section>
  </body>
</html>
```
### Output
![image](https://github.com/user-attachments/assets/e3b05103-b448-4838-a58d-2058d9fe237a)
# Interview Question
### 1.What is the default positioning of an element with position: absolute;? ⭐⭐ */
- **By default, an element with position: absolute; is positioned at the top-left corner of its containing block without any offsets.**
### 2.How can you ensure that an element with position: absolute; is positioned relative to the entire viewport? */
- **To position an element with position: absolute; relative to the viewport, ensure that none of its ancestors have a position property set to relative, absolute, fixed, or sticky. This way, it will use the viewport as its containing block.If we want to move our child dev anywhere then keep that child div into parent div and always parent must be relative and child must be absolute.**
# Fixed (position: fixed;)
- **Elements with position: fixed; are positioned relative to the viewport, so they remain in the same position even when the page is scrolled.**
- **You can use the top, right, bottom, and left properties to specify the exact position.**
### Example-1
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
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
      .main-section {
        width: 100%;
        text-align: center;
        background-color: #1a2980;
        color: #fff;
        display: block;
        box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
          rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
          rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
        /* position fixed start here  */
        position: fixed;
        top: 0;
      }
      #main-heading {
        font-size: 6.2rem;
        margin: 3rem 0;
      }
      .section-full {
        width: 100%;
        height: 100vh;
        background: linear-gradient(to right, #26d0ce, #1a2980);
      }
      .section-full:nth-child(even) {
        background: linear-gradient(to right, #56b4d3, #348f50);
      }
      /* Also again same for the Position Fixed  */
      /* for sticky  */
      .section-full a {
        padding: 16px 32px;
        background-color: #fff;
        color: #1a2980;
        font-size: 24px;
        display: inline-block;
        position: fixed;
        /* position: sticky; */
        top: 50%;
      }
    </style>
  </head>
  <body>
    <div class="main-section">
      <h1 id="main-heading">CSS Positions - Fixed</h1>
    </div>
    <hr />
    <div class="section-full"></div>
    <div class="section-full"><a href="#">Join WhatsApp Now</a></div>
    <div class="section-full"></div>
    <div class="section-full"></div>
  </body>
</html>
```
### Output
![image](https://github.com/user-attachments/assets/259cd149-cab4-41e8-9cd8-6c2142eba449)
# Sticky (position: sticky;)
- **Elements with position: sticky; are initially positioned according to the normal flow, but they become "sticky" and stay within the viewport once they reach a specified scroll position.**
- **You can use the top, right, bottom, and left properties to set the stickiness behavior.**
- **If in any div any element's position is sticky it means it will be sticky in it's position but when that corresponding div will scrrol up or down it's last point then it will also go with the flow of that div**
- **Never,ever it will not sustain when the scroll down or up it's last point.**
> মানে যদি আমরা scroll করার সময় যেই particular div এ যেকোন একটা element এ আমরা position sticky apply করি সেক্ষেত্রে ঐ element টা ততক্ষণ sticky থাকবে যতক্ষণ আমাদের ঐ particular div এর scroll up/down last
> point এ এসে না পৌঁছায়,যখনি সে last point এ এসে div টা পৌছাবে ঠিক তখনি তাকে সাথে করে scroll up/down করে নিয়ে চলে যাবে।

