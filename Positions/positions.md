# Position
![image](https://github.com/user-attachments/assets/5098c9eb-e23c-42b4-b9e9-518e5ce4f3f9)
- **The position property in CSS is used to control the positioning of elements within a web page.**
- **It defines how an element should be placed relative to its normal position in the document flow or relative to its parent or containing elements.**
### Position: relative; 
-- **If we want to move our child dev anywhere then keep that child div into parent div and always parent must be relative and child must be absolute.**
![image](https://github.com/user-attachments/assets/6d40f415-f357-47de-8b07-5a2b55579462)
## Some example of ```parent's position:relative chil'd position:absolute``
/*? Definition: Elements with position: relative; are positioned relative to their normal position in the document flow. */
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
/*? position: absolute; */
/*? Definition: Elements with position: absolute; are positioned relative to the nearest positioned ancestor or the initial containing block. */

