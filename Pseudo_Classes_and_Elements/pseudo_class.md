# Pseudo Class
![image](https://github.com/user-attachments/assets/c49df843-0c46-4244-ab43-b1c395390605)


```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>PSEUDO CLASS IN CSS</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Jost:wght@300;400;500;700&family=Poppins:wght@200;300;400;600&family=Quicksand:wght@300;400;500;600;700&family=Urbanist:wght@300;400;600;700;800;900&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <section class="hero-section">
      <div class="container">
        <div class="grid grid-two-column">
          <div class="hero-content">
            <h1>Best CSS Course Ever</h1>
            <p>
              Unleash your web design potential with the best CSS course on the
              internet! 🚀 Elevate your skills, create stunning websites, and
              transform your career. Join us today and embark on a CSS journey
              like never before.
            </p>
            <a href="https://www.youtube.com/thapatechnical"> watch now </a>
          </div>
          <div class="hero-image">
            <figure>
              <img
                src="../images/css.png"
                alt="headphone with black background"
              />
            </figure>
          </div>
        </div>
      </div>
    </section>
    <!-- 2nd section  -->

    <section class="hero-section section-elements">
      <div class="container">
        <div class="grid grid-two-column">
          <div class="content-1">
            <!-- <!-- <ul> -->
            <p>I am Last</p>
            <p>I am Last</p>
            <p>I am Last</p>
            <li>Home</li>
            <li>Home</li>
            <li>Home</li>
            <li>Home</li>
            <li>Home</li>
            <!--? wht if the p is the last child  -->
            <p>I am Last</p>
            <!-- </ul> -->
          </div>
          <div class="content-2">
            <ul class="testing">
              <li class="p-class">Home</li>
              <li class="p-class">Home</li>
              <li class="p-class">Home</li>
              <li class="p-class">Home</li>
              <li class="p-class">Home</li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </body>
</html>
/*style.css*/
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Jost";
}

body {
  color: azure;
  height: 100vh;
}

.hero-section {
  background-color: #080a0c;
}

.container {
  height: 100vh;
  max-width: 1320px;
  padding: 64px 0;
  margin: 0 auto;
  display: grid;
  align-items: center;
}

.section-elements {
  padding-bottom: 100px;
}

.section-elements .container {
  height: 50vh;
  background-color: #f5f5f5;
  border-radius: 10px;
  -webkit-border-radius: 10px;
  -moz-border-radius: 10px;
  -ms-border-radius: 10px;
  -o-border-radius: 10px;
  color: #080a0c;
}

.grid {
  display: grid;
  align-items: center;
  gap: 6.4rem;
}

.grid-two-column {
  grid-template-columns: repeat(2, 1fr);
}

.hero-content h1 {
  text-align: left;
  font-size: 54px;
}

.hero-content p {
  font-size: 18px;
  letter-spacing: 1px;
  margin: 2rem 0 4rem 0;
}

img {
  max-width: 80%;
  height: auto;
}

.hero-content a {
  background-color: #fff;
  display: inline-block;
  padding: 10px 32px;
  text-transform: capitalize;
  text-decoration: none;
  border-radius: 5px;
  font-size: 24px;
  font-weight: bold;
  -webkit-border-radius: 5px;
  -moz-border-radius: 5px;
  -ms-border-radius: 5px;
  -o-border-radius: 5px;
}

.content-1,
.content-2 {
  text-align: center;
}

li {
  list-style: none;
  font-size: 48px;
}

/*? List of Pseudo Class  */

.hero-content a:link {
  color: rgb(10, 10, 10);
}

.hero-content a:visited {
  color: #d67e03;
}

.hero-content a:hover {
  color: #0062ff;
}

.hero-content a:active {
  color: #f31559;
}

/* .content-1:first-child {
  color: red;
} */

.content-1 ul:first-child {
  color: Red;
}

.content-1 p:first-child {
  color: red;
}

.content-1 p:last-child {
  color: blue;
}


/* .content-1 li:nth-of-type(1) {
  color: red;
} */

/* .content-1 li:first-of-type {
  color: blue;
} */

.content-1 li:last-of-type {
  color: blue;
}

.content-1 li:nth-of-type(2) {
  color: green;
}

.content-1 li:nth-child(odd) {
  color: red;
}

/** ------------------------------------- -->
/** Let's learn something new
/** ---------------------------------------- --> */

.p-class:nth-child(even) {
  color: red;
}


```
- **1. Link (`a:link`): This is the default state for an unvisited link.**
### Output
![image](https://github.com/user-attachments/assets/12b15dc1-9760-43e9-ba6c-33f2e2dd34b4)
- **2. Visited (`a:visited`): This state applies to a link that the user has already visited.**/
### Output
![image](https://github.com/user-attachments/assets/a39aa698-085e-4f40-afac-e6ed7ae0f8fd)

- **3. Hover (`a:hover`): This state triggers when the user hovers their mouse pointer over a link.**
### Output
![image](https://github.com/user-attachments/assets/5d3f5260-3ea4-4011-ab2d-1dc450074fb8)

- **4. Active (`a:active`): This state is triggered when the user clicks on a link.**
### Output
![image](https://github.com/user-attachments/assets/9d94a5f7-f40f-4d92-9072-1d1282437393)

#### LVHA: This acronym represents the order of link states.

- **L for Link (:link): The default state for unvisited links.**
- **V for Visited (:visited): The state for links that the user has already visited.**
- **H for Hover (:hover): The state triggered when the mouse hovers over a link.**
- **A for Active (:active): The state activated when a user clicks on a link.**

### 5.first-child 
- **Selects the first child element of its parent.**
### 6.last-child 
- **Selects the last child element of its parent.**
### 7.nth-child(n(odd/even))
- **Selects elements based on their position within a parent element, where "n" is a numeric value.**
### 8.first-of-type 
- **Selects the first element of its type within its parent.**
### 9.last-of-type
- **Selects the last element of its type within its parent.**
### 10.nth-of-type(n) 
- **Selects elements of a specified type based on their position within a parent.**
### Important Notes
- **The :last-child pseudo-class selects an element if it's the last child within its parent element. It doesn't work if there are other elements after it within the same parent.**
###
- **The :first-child pseudo-class works similarly to :last-child, but it selects the first child element within its parent. Just like :last-child, it will only select an element if it's the first child and not if there are other elements before it within the same parent.**
### Output
![image](https://github.com/user-attachments/assets/348663f2-45a0-4ab2-9d52-19209c6ec553)

 # :is() Pseudo-Class (or :matches()):
- **The :is() pseudo-class allows you to select elements that match any of the provided selectors.**
- **It's particularly useful when you want to apply the same styles to multiple selectors without repeating the styles.**
- **:is() has higher priority than :where().**
- **when we use any element more than 1 times then we will use ```is()```.
- **But in this below example grid is using everywhere that's why we don't use any kind of ```:is()```.But for h1,p,.section-about, .section-testimonial it is not used everywhere that's why we use ```:is()```.
![image](https://github.com/user-attachments/assets/ac4e92a7-f728-4a3a-96d3-54393fdcf610)

# :where() Pseudo-Class:
- **The :where() pseudo-class is similar to :is() and allows you to select elements that match any of the provided selectors.**
- **It's typically used when you want to group selectors without applying specific styles.**
- **:where() has less priority than :is().**
- - **when we use any element more than 1 times then we will use ```where()```.**
- **But in this below example grid is using everywhere that's why we don't use any kind of ```:where()```.But for h1,p,.section-about, .section-testimonial it is not used everywhere that's why we use ```:where()```.**
![image](https://github.com/user-attachments/assets/547bd758-6a79-47e8-bbb2-2bdf1f3b48ea)

# :has() Pseudo-Class:
- **The :has() pseudo-class selects elements that contain a specific element or set of elements that match the provided selector.**
- **It's currently not well-supported in modern browsers and may not be widely used in practice.**

# :not() Pseudo-Class:
- **The :not() pseudo-class allows you to select elements that do not match the provided selector.**
- **It's commonly used to exclude specific elements from being styled.**






































































































































































































































































































































