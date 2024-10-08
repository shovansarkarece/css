# Gradient – CSS
## The linear-gradient() CSS function creates an image consisting of a progressive transition between two or more colors along a straight line 
- **linear-gradient(red, yellow)-->It will always work from top to bottom where first color will be red and second colour will be yellow)**
- **linear-gradient(180deg, red, yellow)-->It will always work from top to bottom where first color will be red and second colour will be yellow)**
- **linear-gradient(to bottom, red, yellow)-->It will always work from top to bottom where first color will be red and second colour will be yellow)**
![image](https://github.com/user-attachments/assets/49452aae-2e71-4bce-82b4-9025d05ae263)
![image](https://github.com/user-attachments/assets/ed81aa83-4ef1-43a0-9238-719d655ded5f)
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
# linear-gradient() with direction
- **linear-gradient(to top, red, yellow)-->It means go towards bottom to top where first color will be red and second colour will be yellow**
- **linear-gradient(360deg, red, yellow)-->It means go towards bottom to top where first color will be red and second colour will be yellow**

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
# linear-gradient() with direction
- **linear-gradient(to left, red, yellow)-->It means go towards left right where first color will be red and second colour will be yellow**
- **linear-gradient(270deg, red, yellow)-->It means go towards left right where first color will be red and second colour will be yellow**
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
- **linear-gradient(to right, red, yellow)-->It means go towards right to left where first color will be red and second colour will be yellow**
- **linear-gradient(90deg, red, yellow)-->It means go towards right to left where first color will be red and second colour will be yellow**
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
- **linear-gradient(to top left, red, yellow)-->It means go towards top left from bottom right first color will be red and second colour will be yellow.**
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
- **linear-gradient(to bottom right, red, yellow);-->It means go towards bottom right from top left first color will be red and second color will be yellow.**
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
- **background-image: linear-gradient(to right, rgba(255, 0, 0, 0), rgba(255, 0, 0, 1));-->> Here, the Last parameter used for transperent** 

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
- **background-image: linear-gradient(
 to right top,
  #051937,
  #004d7a,
  #008793,
  #00bf72,
  #a8eb12);**
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
# Output
![image](https://github.com/user-attachments/assets/9fc2b43e-c741-48e8-89dd-f1d0bd669a70)
# Repeating linear gradient in CSS? 
- **background-image: repeating-linear-gradient(45deg, #d2e0fb, #79ac78 45px);**
- **Here last parameter is 45px which will be repeated the gradient color.**
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
background-image: repeating-linear-gradient(45deg, #d2e0fb, #79ac78 45px);
}
```
# Output
![image](https://github.com/user-attachments/assets/fbad578c-bc11-49f7-8a24-96b6fc89783f)
# Add color overlay on image(Basically using following code to make project)
```
 **background-image: linear-gradient(
    to right top,
    rgba(5, 25, 55, 0.6),//-->a is used for transparency(always use less than 1)
    rgba(0, 77, 122, 0.6),//-->a is used for transparency(always use less than 1)
    rgba(0, 135, 147, 0.6),//-->a is used for transparency(always use less than 1)
    rgba(0, 191, 114, 0.6),//-->a is used for transparency(always use less than 1)
    rgba(168, 235, 18, 0.6)//-->a is used for transparency(always use less than 1)
   ),
   url("https://images.pexels.com/photos/3888151/pexels-photo-3888151.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1");
   background-repeat: no-repeat;
  background-size: cover;**
```
## Example-1
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <!-- <link rel="stylesheet" href="radial-style.css" /> -->
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
      rgba(5, 25, 55, 0.6),
      rgba(0, 77, 122, 0.6),
      rgba(0, 135, 147, 0.6),
      rgba(0, 191, 114, 0.6),
      rgba(168, 235, 18, 0.6)
    ),
    url("https://images.pexels.com/photos/3888151/pexels-photo-3888151.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1");
  background-repeat: no-repeat;
  background-size: cover; 
}
```
# Output
![image](https://github.com/user-attachments/assets/d7b7c44e-d98b-4649-bb3d-5b4c675235d2)


# Explain the difference between linear gradients and radial gradients in CSS. When would you use one over the other?
## Linear gradients create a smooth transition along a straight line, such as from top to bottom or left to right. Radial gradients, on the other hand, create a circular transition from the center outward.We would use linear gradients for linear background effects like horizontal or vertical color transitions. Radial gradients are ideal for creating circular elements or radial backgrounds,such as buttons or circular divs.
# RADIAL GRADIENTS
- **Radial gradients are ideal for creating circular elements or radial backgrounds,such as buttons or circular divs.**
- **The radial-gradient() function sets a radial gradient as the background image.**
- **A radial gradient is defined by its center.**
- **To create a radial gradient you must define at least two color stops.**
- **The shape parameter defines the shape. It can take the value circle or ellipse. The default value is ellipse.**
![image](https://github.com/user-attachments/assets/a9b311ab-b27f-46ab-82f5-3c7ca0da885a)
## Example-1
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="radial-style.css" />
  </head>
  <body>
    <section></section>
  </body>
</html>
////radial-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
section {
  width: 100%;
  height: 100vh;
  background-image: radial-gradient( red, yellow, green);
}
```
## Output
![image](https://github.com/user-attachments/assets/a6224d74-4f01-4930-b058-8596364aacf5)
## Example-2
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="radial-style.css" />
  </head>
  <body>
    <section></section>
  </body>
</html>
////radial-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
section {
  width: 100%;
  height: 100vh;
    background-image: radial-gradient(ellipse, red 20%, yellow 40%, green 40%);
}
```
## Output
![image](https://github.com/user-attachments/assets/f65c5ef1-e892-4c35-bdd8-5ab3df8a1a94)
# Radial Gradient with Shape – CSS
![image](https://github.com/user-attachments/assets/bde3301d-452f-4280-aa41-db3cd1fa4cd1)
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="radial-style.css" />
  </head>
  <body>
    <section></section>
  </body>
</html>
////radial-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
section {
  width: 100%;
  height: 100vh;
     background-image: radial-gradient(circle, red 20%, yellow 40%, green 40%);
}
```
## Output
![image](https://github.com/user-attachments/assets/b5734f9e-b146-42d5-90a3-528445b626f3)
# Repeating radial gradient
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="radial-style.css" />
  </head>
  <body>
    <section></section>
  </body>
</html>
////radial-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
section {
  width: 100%;
  height: 100vh;
     background-image: repeating-radial-gradient(#ff5733, #ffc300, #a8df8e 250px);-->Here 250px is the repeating color
}
```
## Output
![image](https://github.com/user-attachments/assets/de7ddd53-cb58-4c05-aa9d-9512b5def084)
# Circular pattern of colors with smooth transitions between them
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradient Style</title>
    <!-- <link rel="stylesheet" href="linear-style.css" /> -->
    <link rel="stylesheet" href="radial-style.css" />
  </head>
  <body>
    <section></section>
  </body>
</html>
////radial-style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
section {
  width: 100%;
  height: 100vh;
       background: radial-gradient(
    circle at center,
    #ff5733 0%,
    #ffc300 20%,
    #ff5733 40%,
    #2980b9 60%,
    #33ff57 80%,
    #2980b9 100%
  );
}
```
# Output
![image](https://github.com/user-attachments/assets/b3123463-51c8-4038-a342-194b6ad8ad59)
# Disclaimer:
- **In most the cases we are using below link**
- 1)[uigradients](https://uigradients.com/#DIMIGO)
- 2)[cssgradient](https://cssgradient.io/)
- 3)[css-gradient](https://www.css-gradient.com/)
- 4)[mycolor](https://mycolor.space/gradient)
