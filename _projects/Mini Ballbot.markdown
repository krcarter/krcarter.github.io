---
layout: post
title: Mini - Ballbot
description: A self-balancing ball robot.
img: /img/base_render.jpg
---

# Overview
<br />

Spring  2019 capstone project for 16-264 Humanoids Class at Carnegie Mellon University.

The projects was greatly inspired by [Ballbot](https://www.youtube.com/watch?v=8BtDuzu2WeI) a humanoid size robot made in CMU's Microdynamic Systems Laboratory. Instead of balancing on a ball with a 200mm (7.87 inches) diameter we built our robot to balance on a smaller ball with a 95mm (3.75 inches) diameter.

# Base Design
<br />

The base design was design to be an inverse mouse ball mechanism where rollers drive the ball to a specific location. There are four steel rollers surrounding the ball, so it can move in its x or y direction. These rollers are driven by a timing belts attach to a motor with an encoder. For simplicity sakes the body assembly was done with lasered cut acrylic and 3d printed roller bearing assembly. One large bearing is at the center of the assembly for the ball to smoothly roll about.

<img src="http://krcarter.github.io/img/base_render.jpg" alt="base_render" width="350"/> <img src="http://krcarter.github.io/img/miniball_base.png" alt="miniballbase" width="350"/>

# Upper Body
<br />

The upper body is where all the electronics went. To easily create mounting plates we used threaded rods, and this made it easy to attach additional acrylic lasered cut plates to mount the electronics. You will notice that 2 12-volt NiMH batteries are mounted on the very top plate. This was to increase the moment inertia of the pendulum body, for the system will have more time to correct for small disturbances. The rest of the electronics consisted of a simple Arduino Uno, Raspberry Pi for computer vision, and an onboard IMU. 

<img src="http://krcarter.github.io/img/miniUpperReal.jpg" alt="miniUpper" width="300" height ="500"/> <img src="http://krcarter.github.io/img/ballBotIso.png" alt="miniUpperCAD" width="300" height ="500"/>

# Video

Balancing

<iframe width="800" height="533" src="https://www.youtube.com/embed/D2wQ3jEPfwY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Assembly

<iframe width="800" height="533" src="https://www.youtube.com/embed/geEv4d49hWU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
