---
layout: post
title: BB8 Robot
description: A self-balancing ball robot.
img: /img/bb8_title.png
---

## Star Wars BB8 Project
<br />

# Overview
<br />

Back in sophomore year of my undergraduate study at Carnegie Mellon I competed in a week-long build-a-thon known as Build18. During the build-a-thon we were give $300 dollars and told to build something cool for the first week of the spring semester. I decided to recreate a life size version of the popular Star Wars BB8 robot. I was the lead mechanical engineer for the project and work alongside 4 computer science majors to complete the project. The robot during the build-a-thon did not successfully balance at the time, but it did win us some awards. I then went back and reengineered the robot as a case-study in controls senior year in my class, 24-451 Feedback Control Systems.

The projects was greatly inspired by youtuber [James Bruton](https://www.youtube.com/watch?v=dlwcXgZYImU) who does incredible work.

# Chassis
<br />

The chassis was designed with three levels one for the mounting of the motor mounts, another for wiring to the electronics, and the top where the electronics where stored. Each level was made from 1/8" acrylic sheets which could be quickly iterated on with a laser cutter. The acrylic sheets where attach with aluminum standoffs, for if something needed to be reach or changed it can be quickly be done with loosening some bolts. The motor mounts were 3d printed on an Ultimaker and attached with a 2-1/2” long bolt.  

The wheels where 58mm omni-directional wheels to allow holonomic motion on top of the ball. I used four omniwheels instead of possibly three because the math would be easier, and would be simpler to control. Drive motors where 100:1 918d MFA como drill motors that gave a good balance of speed, needed to be fast enough to react to falling, and torque, needed to have enough force to move ball and robot.

<img src="http://krcarter.github.io/img/bb8_iso.png" alt="BB8iso" width="300"/> <img src="http://krcarter.github.io/img/bb8_front.png" alt="BB8front" width="300"/>

# Electronics
<br />

The robot does this using on board sensing with an IMU (inertial measurement unit), beging control by an arduino mega 2560.

# Controls
<br />

# Awards
<br />

For the work we did we won two awards:

1. Lockheed Martin Innovation Award
2. Rockwell Automation Award

