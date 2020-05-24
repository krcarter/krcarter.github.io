---
layout: post
title: The Funky Monkey
description: A swinging monkey Robot.
img: /img/funkeyMonkey_title.png
---

<img src="http://krcarter.github.io/img/funkeyMonkey_title.png" alt="funkyMonkeyTitle" width="644"/>

# Abstract
<br />

Gibbons and similar animals exhibit agile maneuverability with the complex, pendulum-like motion of their legs or tails when swinging from branch to branch (brachiation). Tailed robots developed by Fukuda et al., Chang-Sui et al., and others have each separately shown the robust capabilities tail-like appendages have for modifying robotic movement to improve brachiation and aerial reorientation during a fall. However, a system which combines both of these tail capabilities has yet to be studied. To this end, we developed a bioinspired, three-link swinging robot, in the vein of a triple pendulum, that can modify its motion by means of motor actuation of its lower two links (its tail). By comparing the three-link robot’s ability to swing from rest and reorient in-air to its two-link counterpart, we can study more generally how tails can modify robotic movement, and theoretically gain a better understanding of robotic locomotion. A MATLAB trajectory optimization simulation of the two and three-link robot indicated that a three-link configuration increased maximum achievable velocity while decreasing required torque when swinging from rest. However, during reorientation simulations, the three-link robot required more torque on average to change from a vertical position to a horizontal orientation while falling. Studies conducted with the final prototype were inconclusive with respect to swinging, but seemed to indicate that the three-link configuration was more effective at reorientation. From our experiments we can generally conclude that a tail with greater ability to change its moment of inertia tends to be more effective at robotic motion manipulation, however more testing is required to confirm this fact.

# Final Design
<br />

To effectively change the moment of inertia of our robot, we decided to create a three-link robot with motors between the links, allowing the lower two links to mimic the thigh and shin of a gibbon in what we refer to as the “tail” of the robot. Traditional robots with tails have a single degree of freedom, allowing the tail to simply swing back and forth and providing no ability to instantaneously change the moment of inertia from a hang. Our additional degree of freedom allows our robot more flexibility. We can actuate the motors in opposite directions, creating no rotation of the robot but bringing the center of mass closer to the axis of rotation, thus changing the moment of inertia. Our design allows us to simulate a two-link robot by setting our lower motor to be fixed at an angle of 0°. This allows us to use our robot to compare the performance of a three-link robot versus a two-link one.

Our robot was designed using polycarbonate square tubing for the frame with Dynamixel AX-18A motors connecting the three links. The tubing at the top of the upper link allows the robot to smoothly rotate around the bar of the test stand. The test stand has PTFE tubing between its bar and the robot, creating a very low-friction connection and allowing the robot to closely match our simulated trajectories. To maximize the robot’s ability to change its moment of inertia about the bar, we wanted to maximize the mass in the lower tail of the robot. To do this, we placed the battery at the bottom of the robot and minimized the mass in all other components of the robot. We were able to have more than 40% of the mass of the robot in its bottom link. For all optimization processes see individual technical contributions. The final mass of the robot is 553 g. In the two-link configuration, the robot can reduce its moment of inertia by at most 74%. In the three-link configuration, the robot can reduce its moment of inertia by 85%.

# Project Video
<br />

<iframe width="800" height="533" src="https://www.youtube.com/embed/ONzHTRzSZtE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

