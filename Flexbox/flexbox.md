# FLEXBOX IN CSS
- **Flexbox is a one-dimensional layout model that helps you distribute space along a single axis (either horizontally or vertically) in a flexible and efficient way. It allows you to align and distribute elements within a container, making it easier to create complex layouts without using floats or positioning.**
# Flex Container Properties (Parent) 
![image](https://github.com/user-attachments/assets/b2ccb40a-d802-4396-9c98-86968708f233)

- **1)Flex Container (display: flex;):**
- **To create a flexbox layout, you need a flex container. Apply display: flex; to the container element.**
- Syantax:
```
.flex-container {
     display: flex;
}
```
# Graphical representation of main axis vs cross axis
- **Main Axis and Cross Axis:**
- **In a flex container, one axis is considered the main axis, and the other is the cross axis. You can set the main axis to be either horizontal (row) or vertical (column).**

![image](https://github.com/user-attachments/assets/14ca2d2f-90fc-4e0a-b955-8c8cf8fc1708)

- **2)Flex Direction (flex-direction): Use flex-direction to specify the direction to either main axis or cross-axis.**
![image](https://github.com/user-attachments/assets/6f10ec3b-c695-4ac9-a376-b5e717b80994)

- **Values: row, row-reverse, column, column-reverse.**
- **Items display in a row (the flex-direction property's default is row).**
- **If the flex-direction:row then horizontal will be main-axis.** 
- **if flex-direction:column the vertical part will be main-axis and horizontal axis become the cross axis.**
- Syantax:
```
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```
- **flex-direction:column**

![image](https://github.com/user-attachments/assets/d4697a3c-70ab-4cf6-8134-7a8a681213bc)
- **3)Justify Content (justify-content): justify-content aligns flex items along the main axis means horizentally.**
- **Values include flex-start, flex-end, center, space-between, and space-around.**

![image](https://github.com/user-attachments/assets/35b7c9d2-4eae-4ad3-8b34-63f2a3d4d406)
- **Syntax:**
```
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
}
```
#### Example
- **justify-content: flex-start/start**
 
![image](https://github.com/user-attachments/assets/01703b19-fec1-42cc-b26a-d0df40747f2c)
- **justify-content: center**

![image](https://github.com/user-attachments/assets/dcdf37f9-4d84-4e3d-b13f-3be72105ec7a)
- **justify-content: flex-end/end**

![image](https://github.com/user-attachments/assets/03ee4d59-c85f-4d1a-9916-94f5d3ce8556)
- **justify-content:space-between**
  
![image](https://github.com/user-attachments/assets/b99bd807-df24-4333-b3e0-f7dec0721155)
