# Lists
![image](https://github.com/user-attachments/assets/defb35a2-2aad-4dd2-91f8-a89847f813ef)
## list-style-type:disc;
- **The list-style-type property specifies the type of list item marker.**
## Example-1
```
/*Index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>List in CSS</title>
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
      <div class="lists">
        <ul>
          <li>LIKE</li>
          <li>
            SHARE
            <ul>
              <li>SHARE</li>
              <li>SUBSCRIBE</li>
            </ul>
          </li>
          <li>SUBSCRIBE</li>
        </ul>
      </div>
    </section>
  </body>
</html>
/*style.css*/
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to bottom, #5b697a 0%, #5b697a 50%),
    linear-gradient(to bottom, #fafbfd 0%, #fafbfd 50%);
  background-size: 100% 50%, 100% 50%;
  background-repeat: no-repeat;
  display: grid;
  place-items: center;
}
.lists {
  width: 500px;
  padding: 40px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
}
ul {
  list-style-type: disc;
  /* list-style-type: decimal; */
  /* list-style-position: inside; */
  /* list-style-image: url("../images/mario-run.gif"); */
}

li {
  font-size: 32px;
  font-weight: 400;
  text-transform: capitalize;
  margin-bottom: 16px;
  border: 2px solid #ed5656;
}
```
## Output
![image](https://github.com/user-attachments/assets/bbc26664-efdd-46a9-ac21-b4e3128b12ca)
## list-style-type:circle;
## Example-2
```
/*Index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>List in CSS</title>
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
      <div class="lists">
        <ul>
          <li>LIKE</li>
          <li>
            SHARE
            <ul>
              <li>SHARE</li>
              <li>SUBSCRIBE</li>
            </ul>
          </li>
          <li>SUBSCRIBE</li>
        </ul>
      </div>
    </section>
  </body>
</html>
/*style.css*/
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to bottom, #5b697a 0%, #5b697a 50%),
    linear-gradient(to bottom, #fafbfd 0%, #fafbfd 50%);
  background-size: 100% 50%, 100% 50%;
  background-repeat: no-repeat;
  display: grid;
  place-items: center;
}
.lists {
  width: 500px;
  padding: 40px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
}
ul {
  list-style-type: circle;
  /* list-style-type: decimal; */
  /* list-style-position: inside; */
  /* list-style-image: url("../images/mario-run.gif"); */
}

li {
  font-size: 32px;
  font-weight: 400;
  text-transform: capitalize;
  margin-bottom: 16px;
  border: 2px solid #ed5656;
}
```
## Output
![image](https://github.com/user-attachments/assets/b25fbdde-baa7-469e-9f08-1e8baab8cf93)
## list-style-type:decimal;
## Example-3
```
/*Index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>List in CSS</title>
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
      <div class="lists">
        <ul>
          <li>LIKE</li>
          <li>
            SHARE
            <ul>
              <li>SHARE</li>
              <li>SUBSCRIBE</li>
            </ul>
          </li>
          <li>SUBSCRIBE</li>
        </ul>
      </div>
    </section>
  </body>
</html>
/*style.css*/
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to bottom, #5b697a 0%, #5b697a 50%),
    linear-gradient(to bottom, #fafbfd 0%, #fafbfd 50%);
  background-size: 100% 50%, 100% 50%;
  background-repeat: no-repeat;
  display: grid;
  place-items: center;
}
.lists {
  width: 500px;
  padding: 40px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
}
ul {
  list-style-type: decimal; 
}
li {
  font-size: 32px;
  font-weight: 400;
  text-transform: capitalize;
  margin-bottom: 16px;
  border: 2px solid #ed5656;
}
```
## Output
![image](https://github.com/user-attachments/assets/485d2c5d-05af-49d1-b9a8-891696876e7c)
## list-style-type:lower-roman;
## Example-4
```
/*Index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>List in CSS</title>
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
      <div class="lists">
        <ul>
          <li>LIKE</li>
          <li>
            SHARE
            <ul>
              <li>SHARE</li>
              <li>SUBSCRIBE</li>
            </ul>
          </li>
          <li>SUBSCRIBE</li>
        </ul>
      </div>
    </section>
  </body>
</html>
/*style.css*/
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to bottom, #5b697a 0%, #5b697a 50%),
    linear-gradient(to bottom, #fafbfd 0%, #fafbfd 50%);
  background-size: 100% 50%, 100% 50%;
  background-repeat: no-repeat;
  display: grid;
  place-items: center;
}
.lists {
  width: 500px;
  padding: 40px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
}
ul {
  list-style-type: lower-roman; 
}
li {
  font-size: 32px;
  font-weight: 400;
  text-transform: capitalize;
  margin-bottom: 16px;
  border: 2px solid #ed5656;
}
```
## Output
![image](https://github.com/user-attachments/assets/d0a56623-ed81-40d7-aec0-67b506332758)
## list-style-type:upper-roman;
## Example-5
```
/*Index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>List in CSS</title>
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
      <div class="lists">
        <ul>
          <li>LIKE</li>
          <li>
            SHARE
            <ul>
              <li>SHARE</li>
              <li>SUBSCRIBE</li>
            </ul>
          </li>
          <li>SUBSCRIBE</li>
        </ul>
      </div>
    </section>
  </body>
</html>
/*style.css*/
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to bottom, #5b697a 0%, #5b697a 50%),
    linear-gradient(to bottom, #fafbfd 0%, #fafbfd 50%);
  background-size: 100% 50%, 100% 50%;
  background-repeat: no-repeat;
  display: grid;
  place-items: center;
}
.lists {
  width: 500px;
  padding: 40px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
}
ul {
  list-style-type:upper-roman;
li {
  font-size: 32px;
  font-weight: 400;
  text-transform: capitalize;
  margin-bottom: 16px;
  border: 2px solid #ed5656;
}
```
## Output
![image](https://github.com/user-attachments/assets/46ff8702-686e-48e2-a142-9e7ee0451a4b)
## list-style-type:lower-alpha/lower-latin
## Example-6
```
/*Index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>List in CSS</title>
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
      <div class="lists">
        <ul>
          <li>LIKE</li>
          <li>
            SHARE
            <ul>
              <li>SHARE</li>
              <li>SUBSCRIBE</li>
            </ul>
          </li>
          <li>SUBSCRIBE</li>
        </ul>
      </div>
    </section>
  </body>
</html>
/*style.css*/
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to bottom, #5b697a 0%, #5b697a 50%),
    linear-gradient(to bottom, #fafbfd 0%, #fafbfd 50%);
  background-size: 100% 50%, 100% 50%;
  background-repeat: no-repeat;
  display: grid;
  place-items: center;
}
.lists {
  width: 500px;
  padding: 40px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
}
ul {
  list-style-type:lower-alpha/lower-latin;
li {
  font-size: 32px;
  font-weight: 400;
  text-transform: capitalize;
  margin-bottom: 16px;
  border: 2px solid #ed5656;
}
```
## Output
![image](https://github.com/user-attachments/assets/eaa99ab7-869d-4180-8781-f4b04b150d25)
## list-style-type:upper-latin/upper-alpha;
## Example-7
```
/*Index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>List in CSS</title>
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
      <div class="lists">
        <ul>
          <li>LIKE</li>
          <li>
            SHARE
            <ul>
              <li>SHARE</li>
              <li>SUBSCRIBE</li>
            </ul>
          </li>
          <li>SUBSCRIBE</li>
        </ul>
      </div>
    </section>
  </body>
</html>
/*style.css*/
html {
  font-family: "Urbanist";
}
body {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to bottom, #5b697a 0%, #5b697a 50%),
    linear-gradient(to bottom, #fafbfd 0%, #fafbfd 50%);
  background-size: 100% 50%, 100% 50%;
  background-repeat: no-repeat;
  display: grid;
  place-items: center;
}
.lists {
  width: 500px;
  padding: 40px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
}
ul {
  list-style-type:upper-latin/upper-alpha;
li {
  font-size: 32px;
  font-weight: 400;
  text-transform: capitalize;
  margin-bottom: 16px;
  border: 2px solid #ed5656;
}
```
## Output
![image](https://github.com/user-attachments/assets/a4f5bf5d-6402-43e4-92b2-e0ffdaa7c0f2)

/*? The list-style-image property specifies an image as the list item marker: */

/*? The list-style-position property specifies the position of the list-item markers (bullet points). */

/*? The list-style property is a shorthand property. It is used to set all the list properties in one declaration: */
