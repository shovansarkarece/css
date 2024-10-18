# Box Model
![image](https://github.com/user-attachments/assets/e333b140-e28b-4e16-b438-978502f1d4b1)
##### The CSS Box Model consists of four main components:
- **1)Content: This is the innermost part of the element, which holds the actual content, such as text, images, or other HTML elements.**

- **2)Padding: Padding is the space between the content and the element's border. It provides internal spacing within the element.**
            content and border ke bix ka space ko padding 
    
- **3)Border: The border surrounds the padding and content, creating a visible boundary around the element. It can have a thickness, style, and color.**

- **4)Margin: The margin is the space outside the element's border. It separates the element from other elements on the page and controls the spacing between elements.**

##### VERY VERY IMPORTANT

- **CSS box-sizing is a property that controls how the total width and height of an element are calculated, including its content, padding, and border.**
- **It has two possible values: content-box (default) and border-box**

#### box-sizing: content-box:
- **In the default content-box value, an element's width and height are calculated based on its content area. Padding and border are added to the specified width and height.**
- **This means that if you set the width of an element to 100 pixels, and then add 10 pixels of padding and a 2-pixel border, the element's total width will be 100 + 10 + 2 = 112 pixels.**

#### box-sizing: border-box:
- **When using border-box, an element's width and height include its content, padding, and border. Padding and border are subtracted from the specified width and height.**
- **In this case, if you set the width of an element to 100 pixels, and then add 10 pixels of padding and a 2-pixel border, the content area will be adjusted to fit within the specified 100-pixel width, and the padding and border are contained within that.**

#  MARGIN IN CSS 
- **The `margin` property defines the space outside the element's border. It creates separation between the element and other elements in the layout.**
- **Margins create extra space around an element, unlike padding, which creates extra space within an element.**
- **SYNTAX:**
### Four Values: `margin: top right bottom left;`**
- **margin: 50px 40px 30px 60px;**
- **`top`: Specifies the margin on the top side.**
- **`right`: Specifies the margin on the right side.**
- **`bottom`: Specifies the margin on the bottom side.**
- **`left`: Specifies the margin on the left side.**
### Four Values: `margin: top right bottom left;`
 - **`margin: 200px 200px 200px 200px;`**
### Three Values: margin: top right-left bottom;
- **margin: 50px 30px 60px;**
- **`top`: Specifies the margin on the top side.**
- **`right-left`: Specifies the margin on the right and left sides.**
- **`bottom`: Specifies the margin on the bottom side.**
### Three Values: `margin: top right-left bottom;`
 - **`margin: 100px 200px 150px;`**
### Two Values: margin: top-bottom right-left; */
- **margin: 50px 30px;**
- **`top-bottom`: Specifies the margin on the top and bottom sides.**
- **`right-left`: Specifies the margin on the right and left sides.**
### Two Values: `margin: top-bottom right-left;`
- **`margin: 100px 200px;`**
### One Value: `margin: value;`
- **`margin: 50px;`**
- **If you provide a single value, it applies to all sides equally.**
