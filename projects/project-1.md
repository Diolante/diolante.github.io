---
layout: project
type: project
image: images/micromouse.jpg
title: Matching Template with K-Means for Rhizobia Nodes Detection
permalink: projects/matchingRhizobia
# All dates must be YYYY-MM-DD format!
date: 2019-12-01
labels:
  - Image Processing
  - K-Means
  - Python
  - Rhizobium 
summary: A small project to detect rhizobium nodes in legumes roots using OpenCV and K-Means.
---

<div class="ui small rounded images">
  <img class="ui image" src="https://raw.githubusercontent.com/Diolante/Matching-Template-with-K-Means-for-Rhizobia-Nodes-Detection/master/Exp.1%20-%20Florest%C3%B3polis%2C%2035DAE%2C%202017-2018%2C%20T15%2C%20R1%2C%20P2.jpg">
  <img class="ui image" src="https://raw.githubusercontent.com/Diolante/Matching-Template-with-K-Means-for-Rhizobia-Nodes-Detection/master/Exp.1%20-%20Florest%C3%B3polis%2C%2035DAE%2C%202017-2018%2C%20T22%2C%20R5%2C%20P3.jpg">
  <img class="ui image" src="https://raw.githubusercontent.com/Diolante/Matching-Template-with-K-Means-for-Rhizobia-Nodes-Detection/master/Exp.2%20-%20Florest%C3%B3polis%2C%2035DAE%2C%202017-2018%2C%20T4%2C%20R2%2C%20P4.jpg">
</div>

Micromouse is an event where small robot “mice” solve a 16 x 16 maze.  Events are held worldwide.  The maze is made up of a 16 by 16 gird of cells, each 180 mm square with walls 50 mm high.  The mice are completely autonomous robots that must find their way from a predetermined starting position to the central area of the maze unaided.  The mouse will need to keep track of where it is, discover walls as it explores, map out the maze and detect when it has reached the center.  having reached the center, the mouse will typically perform additional searches of the maze until it has found the most optimal route from the start to the center.  Once the most optimal route has been determined, the mouse will run that route in the shortest possible time.

For this project, I was the lead programmer who was responsible for programming the various capabilities of the mouse.  I started by programming the basics, such as sensor polling and motor actuation using interrupts.  From there, I then programmed the basic PD controls for the motors of the mouse.  The PD control the drive so that the mouse would stay centered while traversing the maze and keep the mouse driving straight.  I also programmed basic algorithms used to solve the maze such as a right wall hugger and a left wall hugger algorithm.  From there I worked on a flood-fill algorithm to help the mouse track where it is in the maze, and to map the route it takes.  We finished with the fastest mouse who finished the maze within our college.

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse Website](http://www-ee.eng.hawaii.edu/~mmouse/about.html).



