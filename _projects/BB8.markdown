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

<img src="http://krcarter.github.io/img/bb8_ball.png" alt="BB8ball" width="300"/>

# Electronics
<br />

To get the robot to balance I always needed the robot to know its orientation, and to do this I need to use an IMU (inertial measurement unit). My IMU of choice was the SparkFun 9Dof IMU Breakout – LSM9DS1. This board was easy to wire using its i2c protocol. Also, it measured acceleration and angular rate of change in x-y-z and roll-pitch-yaw which was perfect for mt application. The embedded board I used was an Arduino Mega 2560 it was perfect for getting the robot up and running as fast as possible. The motors were controlled by two Pololu – Dual VNH2SP30 motor driver carrier which took PWM signals and powered the motors.

# Controls
<br />

To have the robot self-balance was a straight forward application of PID feedback control. I sampled the robot orientation from the IMU every 10 ms along the roll and pitch axis from the gyroscope and accelerometer. I needed both gyroscope and accelerometer data because even though the gyroscope was accurate its data slipped over time. The accelerometer could not be used by itself because there was a lot of noise coming from every little force the accelerometer experience. To combine both sensing devices I used a complementary filter. The complementary filter uses 98% of the gyro data and 2% of the accelerometer data to stop drifting. You can read more about it [here](http://www.pieter-jan.com/node/11). 

The complimentary returned a degree value which was a small angle less than 5 degrees. The error of the control was how far this value was away from zero. Tuning the PID controller I was able to get a balancing robot.

<img src="http://krcarter.github.io/img/blkdiagram.png" alt="blkdiagram" width="600"/>
# Awards
<br />

For the work we did we won two awards:

1. Lockheed Martin Innovation Award
2. Rockwell Automation Award

