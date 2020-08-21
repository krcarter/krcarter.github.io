---
layout: post
title: Mini - Ballbot
description: A self-balancing ball robot.
img: /img/base_render.jpg
---

# Overview
<br />

Spring  2019 capstone project for 16-264 Humanoids Class at Carnegie Mellon University.

The projects was greatly inspired by [Ballbot](https://www.youtube.com/watch?v=8BtDuzu2WeI) a humanoid size robot made in CMU's Microdynamic Systems Laboratory

# Base Design
<br />

The chassis was designed with three levels one for the mounting of the motor mounts, another for wiring to the electronics, and the top where the electronics where stored. Each level was made from 1/8" acrylic sheets which could be quickly iterated on with a laser cutter. The acrylic sheets where attach with aluminum standoffs, for if something needed to be reach or changed it can be quickly be done with loosening some bolts. The motor mounts were 3d printed on an Ultimaker and attached with a 2-1/2” long bolt.  

The wheels where 58mm omni-directional wheels to allow holonomic motion on top of the ball. I used four omniwheels instead of possibly three because the math would be easier, and would be simpler to control. Drive motors where 100:1 918d MFA como drill motors that gave a good balance of speed, needed to be fast enough to react to falling, and torque, needed to have enough force to move ball and robot.

<img src="http://krcarter.github.io/img/base_render.jpg" alt="base_render" width="400"/>
