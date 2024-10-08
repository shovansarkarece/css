# DROP SHADOW
- **Drop shadow, often used for images, creates a shadow below the element, giving the illusion of it being lifted from the page.** 
- **It is defined using the filter property with the drop-shadow function.**
- **The drop-shadow function accepts values for horizontal and vertical offsets, blur radius, and color.**
- 
![image](https://github.com/user-attachments/assets/4e7e126b-bab4-457d-813b-95beda942453)

## values  
- **Two length values**
- **(i)drop-shadow(``` <length> <length> ```)**
- **(ii)drop-shadow(5px 5px)**
- **Three length values**
- **(i)drop-shadow(``` <length> <length> <length> ```)**
- **(ii)drop-shadow(5px 5px 15px)**
- **Two length values and a color**
- **(i)drop-shadow(``` <length> <length> <color> ```)**
- **(ii)drop-shadow(5px 5px yellow)**

- **Three length values and a color**
- **(i)drop-shadow(``` <length> <length> <length> <color> ```)**
- **(ii)drop-shadow(5px 5px 15px yellow)**

- **The order of color and length values can be changed**
- **(i)drop-shadow(``` <color> <length> <length> <length> ```)**
- **(ii)drop-shadow(#e23 0.5rem 0.5rem 1rem)**
## Example-1(blur-radius with color)
```
//////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Drop shadow</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../../images/brand.png" alt="marketing company" />
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
body {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  background-color: black;
  display: grid;
  place-items: center;
}
img {
   filter:drop-shadow(0 0 10px #fff);////3rd parameter is for blur-radius with color
}
```
## Output
![image](https://github.com/user-attachments/assets/962a02ba-9a99-411e-9ddd-a8043c817618)
## Example-2(blur-radius with color)
```
//////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Drop shadow</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../../images/brand.png" alt="marketing company" />
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
body {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  background-color: black;
  display: grid;
  place-items: center;
}
img {
   filter:drop-shadow(0 0 10px #fff);////3rd parameter is for blur-radius with color
}
```
## Output
![image](https://github.com/user-attachments/assets/85aa0bbd-d190-428a-9934-dcecb457b384)
## Example-3(Offset-X,Offset-Y,color)
```
//////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Drop shadow</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../../images/brand.png" alt="marketing company" />
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
body {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  background-color: black;
  display: grid;
  place-items: center;
}
img {
   filter: drop-shadow(-10px 10px 0px #f90000);////(Offset-X,Offset-Y,without blur-radius,color
}
```
## Output
![image](https://github.com/user-attachments/assets/0b2a8c2c-9dea-4cc0-88cc-b7314690da97)

## Example-4(Offset-X,Offset-Y,blur-radius,color)
```
//////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Drop shadow</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section>
      <img src="../../images/brand.png" alt="marketing company" />
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
body {
  width: 100%;
  height: 100vh;
  background-color: hsl(0, 0%, 94%);
  background-color: black;
  display: grid;
  place-items: center;
}
img {
   filter: drop-shadow(-10px 10px 10px #f90000);////(Offset-X,Offset-Y,blur-radius,color)
}
```
## Output
![image](https://github.com/user-attachments/assets/edf01a3e-8699-4152-a01f-770d67d3e74c)
