# Gradient – CSS
## The linear-gradient() CSS function creates an image consisting of a progressive transition between two or more colors along a straight line 
- **linear-gradient(red, yellow)-->It will always work from top to bottom)**
  
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
}
```
## Output
### linear-gradient(red, yellow)-->It will always work from top to bottom)
# Gradient with Direction – CSS
## linear-gradient(to left, red, yellow)-->It means go towards left right where first color will be red and second colour will be yellow
![image](https://github.com/user-attachments/assets/6f6f8142-3d94-4eae-bf7c-9252befad9ea)
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
}
```
## Output
![image](https://github.com/user-attachments/assets/42f20741-5895-4c3d-972f-7b0a4950844d)
## Example-3
## linear-gradient(to top, red, yellow)-->It means go towards bottom to top where first color will be red and second colour will be yellow
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
}
```
## Output
![image](https://github.com/user-attachments/assets/bcbccc24-3bd8-4a84-bec7-e4d9ec103f61)

# Gradient with Angles – CSS
![image](https://github.com/user-attachments/assets/f05f0314-eafb-49b7-bf65-61e98c349b38)
# Radial Gradient – CSS 
![image](https://github.com/user-attachments/assets/a9b311ab-b27f-46ab-82f5-3c7ca0da885a)
# Gradient with Shape – CSS
![image](https://github.com/user-attachments/assets/b03b37ab-966e-47db-9435-ebd64e637d05)
