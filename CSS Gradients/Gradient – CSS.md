# Gradient – CSS
## The linear-gradient() CSS function creates an image consisting of a progressive transition between two or more colors along a straight line 
- **linear-gradient(red, yellow)-->It will always work from top to bottom where first color will be red and second colour will be yellow)**
- **linear-gradient(180deg, red, yellow)-->It will always work from top to bottom where first color will be red and second colour will be yellow)**
- **linear-gradient(to bottom, red, yellow)-->It will always work from top to bottom where first color will be red and second colour will be yellow)**
![image](https://github.com/user-attachments/assets/49452aae-2e71-4bce-82b4-9025d05ae263)
## Example-1
```
////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="linear-style.css"> 
  </head>
  <body>
    <section></section>
  </body>
</html>
////linear-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

section {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(red, yellow);
  background-image:linear-gradient(180deg, red, yellow)
  background-image: linear-gradient(to bottom, red, yellow);
}
```
## Output
![image](https://github.com/user-attachments/assets/2ca72867-f245-4af1-9599-f6e119e0be69)
## linear-gradient(to top, red, yellow)-->It means go towards bottom to top where first color will be red and second colour will be yellow
## linear-gradient(360deg, red, yellow)-->It means go towards bottom to top where first color will be red and second colour will be yellow
![image](https://github.com/user-attachments/assets/6f6f8142-3d94-4eae-bf7c-9252befad9ea)
## Example-2
```
////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="linear-style.css"> 
  </head>
  <body>
    <section></section>
  </body>
</html>
////linear-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

section {
  width: 100%;
  height: 100vh;
 background-image: linear-gradient(to top, red, yellow);
    /* background-image: linear-gradient(360deg, red, yellow); */
}
```
## Output
![image](https://github.com/user-attachments/assets/76409802-48b3-4b26-b74b-413777f3b79c)
# Gradient with Direction – CSS
## linear-gradient(to left, red, yellow)-->It means go towards left right where first color will be red and second colour will be yellow
## linear-gradient(270deg, red, yellow)-->It means go towards left right where first color will be red and second colour will be yellow
## Example-1
```
////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="linear-style.css"> 
  </head>
  <body>
    <section></section>
  </body>
</html>
////linear-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

section {
  width: 100%;
  height: 100vh;
 background-image: linear-gradient(to left, red, yellow);
}
```
## Output
![image](https://github.com/user-attachments/assets/9004a835-9593-4655-9531-39b38832dbab)
## Example-2
## linear-gradient(to right, red, yellow)-->It means go towards right to left where first color will be red and second colour will be yellow
## linear-gradient(90deg, red, yellow)-->It means go towards right to left where first color will be red and second colour will be yellow 
![image](https://github.com/user-attachments/assets/6f6f8142-3d94-4eae-bf7c-9252befad9ea)
```
////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="linear-style.css"> 
  </head>
  <body>
    <section></section>
  </body>
</html>
////linear-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

section {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(to right, red, yellow);
  background-image: linear-gradient(90deg, red, yellow);
}
```
## Output
![image](https://github.com/user-attachments/assets/42f20741-5895-4c3d-972f-7b0a4950844d)
# Gradient with Diagonal Direction
## Example-1
## linear-gradient(to top left, red, yellow)-->It means go towards top left from bottom right first color will be red and second colour will be yellow.
```
////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="linear-style.css"> 
  </head>
  <body>
    <section></section>
  </body>
</html>
////linear-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

section {
  width: 100%;
  height: 100vh;
 background-image: linear-gradient(to top left, red, yellow);
}
```
## Output
![image](https://github.com/user-attachments/assets/221c2cf2-43e3-4197-b377-42aecfe90f7f)
## Example-2
## linear-gradient(to bottom right, red, yellow);-->It means go towards bottom right from top left first color will be red and second color will be yellow.
```
////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="linear-style.css"> 
  </head>
  <body>
    <section></section>
  </body>
</html>
////linear-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

section {
  width: 100%;
  height: 100vh;
 background-image: linear-gradient(to bottom right, red, yellow);
}
```
## Output
![image](https://github.com/user-attachments/assets/e25f9ed5-0912-4b9d-b884-09bf000d13f8)
## 4: How can you create a transparent gradient in CSS? 🚀 
### background-image: linear-gradient(to right, rgba(255, 0, 0, 0), rgba(255, 0, 0, 1)); 
```
////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="linear-style.css"> 
  </head>
  <body>
    <section></section>
  </body>
</html>
////linear-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

section {
  width: 100%;
  height: 100vh;
 background-image: linear-gradient(to right, rgba(255, 0, 0, 0), rgba(255, 0, 0, 1));
}
```
# Output
![image](https://github.com/user-attachments/assets/ea16794e-c7b6-44b9-8f78-bf30caff990d)
# transitions from multiple colors rather than just two
  background-image: linear-gradient(
 to right top,
  #051937,
  #004d7a,
  #008793,
  #00bf72,
  #a8eb12);
```
////index.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="linear-style.css"> 
  </head>
  <body>
    <section></section>
  </body>
</html>
////linear-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

section {
  width: 100%;
  height: 100vh;
  background-image: linear-gradient(
    to right top,
    #051937,
    #004d7a,
    #008793,
    #00bf72,
    #a8eb12
  );
}
```


# Explain the difference between linear gradients and radial gradients in CSS. When would you use one over the other?
## Linear gradients create a smooth transition along a straight line, such as from top to bottom or left to right. Radial gradients, on the other hand, create a circular transition from the center outward. 
## You would use linear gradients for linear background effects like horizontal or vertical color transitions. Radial gradients are ideal for creating circular elements or radial backgrounds, 
## such as buttons or circular divs.*/

# Radial Gradient – CSS 
![image](https://github.com/user-attachments/assets/a9b311ab-b27f-46ab-82f5-3c7ca0da885a)
# Gradient with Shape – CSS
![image](https://github.com/user-attachments/assets/b03b37ab-966e-47db-9435-ebd64e637d05)
