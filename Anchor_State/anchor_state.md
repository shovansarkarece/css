# Anchor_State
![image](https://github.com/user-attachments/assets/17b0c595-2b7e-4ba2-b30e-32fdcd5315cf)
## Link (```a:link```)
- **1. Link(```a:link```): This is the default state for an unvisited link.**
## Example-1
```
/*index.html*/
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>ANCHOR STYLING</title>
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
            <h1>World Best CSS Course</h1>
            <p>
              Unleash your web design potential with the best CSS course on the
              internet! 🚀 Elevate your skills, create stunning websites, and
              transform your career. Join us today and embark on a CSS journey
              like never before.
            </p>
            <a href="https://www.youtube.com/thapatechnical" target="_blank">
              watch now
            </a>
          </div>
          <div class="hero-image">
            <figure>
              <img
                src="../images/hero.png"
                alt="headphone with black background"
              />
            </figure>
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
  background-color: #080a0c;
  color: azure;
  height: 100vh;
}

.container {
  height: 100vh;
  max-width: 1320px;
  padding: 64px 0;
  margin: 0 auto;
  display: grid;
  align-items: center;
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
  width: 100%;
  height: auto;
}

.hero-content a {
  color: #080a0c;
}
.hero-content a:link {
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
.hero-content a:visited {
  color: #d67e03;
}
.hero-content a:hover {
  color: #0062ff;
}

.hero-content a:active {
  color: #f31559;
}
```
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

#### LVHA: This acronym represents the order of link states. */

- **L for Link (:link): The default state for unvisited links.**
- **V for Visited (:visited): The state for links that the user has already visited.**
- **H for Hover (:hover): The state triggered when the mouse hovers over a link.**
- **A for Active (:active): The state activated when a user clicks on a link.**

>We can remember the order by recalling the word "LVHA," which represents the sequence of link states. This can help us to remember the order and apply styles more easily in your CSS.
