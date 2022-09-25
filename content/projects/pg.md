---
title: "First attempt at Ray Tracing and Bezier Curves"
date: 2022-09-21T11:08:26-03:00
draft: false
---

Last semester I took a course in Computer Graphics. It was mostly Linear Algebra, which made me feel right at home. My baggage as a former Physics student made it so that almost all the mathematics was quite easy. I could focus more on implement my group's project, which I did almost all by myself.

There were two projects: a ray tracing engine and a bezier curves engine.

## Ray Tracing

The code for this project can be found [here](https://github.com/marvmelo/ray-tracing).

The idea of ray tracing is to shoot several light rays from the camera through the screen and calculate the effects that the light bouncing around the scene has. My implementation allows for and arbritary number of objects (spheres and planes) to be rendered with any color configuration possible using Phong Shading, reflection and transparency.

The image below was my favorite. I rendered two semi-transparent spheres with high refraction angles in a box of mirrors and one single light source. It took about 20 minutes to render (Python was not the best choice).
![Ray Tracing](/img/raytracing.jpg)

## Bezier Curves

The second project I had to implement was a bezier curves visualizer. The code can be found [here](https://github.com/marvmelo/bezier-curves).

I had to do this completely by myself. In the case of ray tracing, my team mates wrote an ealier version of the code that evolved into spaghetti and had to be rewritten. That means that, although the final code was entirely written by me, I can't say I did it all alone. But for the bezier curves project, none of them managed to write a single line of code.

The idea of bezier curves is to use [De Casteljau's Algorithm](https://en.wikipedia.org/wiki/De_Casteljau%27s_algorithm) to calculate the curve whose points are a interpolation of the given control points. In my implementation, the curve is actually approximated by several small lines.

My application is able to render an arbitrary number of bezier curves and change their control points. I used pygame for convenience. The image below shows two bezier curvers and their control points.
![Bezier Curves](/img/bezier.png)

## What now?

I am currently working on a way to combine the two projects. My goal is to be able to render arbitrary bezier surfaces with ray tracing. This new endeavor is being written in C++ due to performance reasons. Unfortunately, I have not been able to progress a lot because of my number of classes. I hope I can finish it in November, when I will be on vacations.