# Workshop-0

Link: [https://whosaidthat-3636.github.io/Workshop-0/]

In this workshop, the idea is the experiment with different variables, conditions and increments through 2D primitives

## Tasks
* Create a p5.js editorLinks to an external site. login and sign up to the Processing Foundation's forumLinks to an external site
* Make a p5.js sketch using 2D primitive shapes, variables, and conditionals. Make sure to save your work.
* Experiment with at least one of the following 2D primitive shapes from the p5.js documentation: line, triangle, quad, arc.
* Keep notes to clearly document your process and learning.

### 1. Setting up the canvas and 2D shapes
- Background
  * setting the scale of the Canvas to be 300 in width, 400 in height
  * background selected from a [RGB color picker](https://www.rapidtables.com/web/color/RGB_Color.html) to be a lighter shade closer to white
  ```
  function setup() {
  createCanvas(300, 400);}
  function draw() {
  background(250, 249, 249);
- Lines
  * straight line
  * lines at an angle
  * heavier strokes 
  ```
  stroke(0);
  strokeWeight(5);
  line(250, 15, 400, 15);
  line(150, 90, 400, 20);
  line(180, 150, 400, 60);
  ```
- Arc
  * placed in the middle of the canvas
  * with no fill
  ```
  noStroke();
  fill(204, 204, 255);
  arc(155, 280, 100, 100, 0, PI + HALF_PI);
  ```
- Triangle
  * placed at the top left of the canvas
  ```
  noStroke(0);
  fill(153, 204, 244);
  triangle(15, 25, 155, 10, 30, 250);
  ```
- Rectangle
  * placed on the right of the canvas
  * half of the shape is out of the canvas view
  * with a white stroke
  ```
  stroke(255);
  fill(255, 255, 153);
  rect(250, 100, 100, 200);
  ```

### 2. Arc
- I started with the color through a [RGB color picker](https://www.rapidtables.com/web/color/RGB_Color.html)
- The arc has a parameter that allows for a specific mode to fill the arc. For this instance a quarter has been taken off a full circle through the parameters of "PI + HALF_PI"
- The idea is to have the arc go in a loop using assignment by using a variable, expression and condition followed by the workshop video
   <img width="572" alt="image" src="https://github.com/user-attachments/assets/3d520f14-20ea-4958-94b9-628583862305" />

- However the code does not work because the shape moves in the _left direction_ but is _set to reset on the left side_ of the canvas 
 ```

  x = x - 6; 

  if (x > width) { 

    x = 100;}
```
- 




  
  




