# Container Queries
- **Container queries enable you to apply styles to an element based on the size of the element's container.**
- **container-type: The container-type CSS property is used to define the type of containment used in a container query.**
- **Syntax:**
```
container-type: normal;
container-type: size;
container-type: inline-size; 
```
![image](https://github.com/user-attachments/assets/f11bfdd1-771f-4fc6-a5e8-c8335cea355c)
![image](https://github.com/user-attachments/assets/a2c88188-091f-4136-8f1b-ee037498eaf3)
# Example
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>container queries</title>
    <style>
      * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: "urbanist";
      }
      body {
        height: 100vh;
        background-color: #191717;
      }
      .container,
      .media {
        max-width: 800px;
        height: auto;
        border: 5px solid #ffb000;
        margin-right: 200px;
        & div {
          display: grid;
          grid-template-columns: 1fr 0.5fr;
          align-items: center;
        }
      }
      .container {
        container-type: inline-size;
        container-name: changelayout;
      }
      img {
        width: 100%;
        height: auto;
      }
      h1 {
        text-align: center;
        color: #fff;
        font-weight: bold;
        text-transform: capitalize;
        font-size: 32px;
        text-shadow: -3px 10px 10px rgba(249, 141, 141, 0.2);
        animation: floating 2s linear infinite alternate;
      }
      @container changelayout (width <= 600px) {
        .container div {
          grid-template-columns: 1fr;
        }
        h1 {
          color: #ffb000;
          text-transform: uppercase;
          padding: 20px 0;
        }
      }
      @media (width <= 600px) {
        .media div {
          grid-template-columns: 1fr;
        }
        h1 {
          color: #ffb000;
          text-transform: uppercase;
          padding: 20px 0;
        }
      }
    </style>
  </head>
  <body>
    <br /><br />
    <div class="container">
      <div>
        <img src="../../images/html.png" alt="" />
        <h1>new css feature container queries..</h1>
      </div>
    </div>
    <br /><br />
    <div class="media">
      <div>
        <img src="../../images/html.png" alt="" />
        <h1>new css feature container queries..</h1>
      </div>
    </div>
  </body>
</html>
```
