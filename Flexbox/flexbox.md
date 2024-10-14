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
- **Values: row, row-reverse, column, column-reverse.**
- **If the flex-direction:row then horizontal will be main-axis.** 
- **if flex-direction:column the vertical part will be main-axis and horizontal axis become the cross axis.**
- Syantax:
```
.flex-container {
  flex-direction: row; /* Horizontal main axis (default) */
}
```
- **flex-direction:column**

![image](https://github.com/user-attachments/assets/d4697a3c-70ab-4cf6-8134-7a8a681213bc)
