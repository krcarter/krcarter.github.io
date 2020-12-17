---
layout: post
title: Research - Gazebo
description: Powered Passive Walking Simulator
img: /img/wobblyB.png
---

# Overview
<br />

I am very interested in studying legged locomotion, and more specifically bipedal legged locomotion. One of the earliest and simplest paradigms to studying legged locomotion is studying the passive dynamic model that was established in the 80s by Professor Tad McGeer. This model of walking breaks the walking problem to its simplest form. Later, the compass-gait model of walking studied by Professor Andy Ruina at Cornell established a model where walking was an energy conservation between a robot’s stance and swing leg walking down a ramp. To learn more read about [Passive Dynamic Walking](https://en.wikipedia.org/wiki/Passive_dynamics) on Wikipedia

<p align="center">
  <img src="http://krcarter.github.io/img/passive.png" alt="passive Walking" width="400"/>
</p>

<p align="center">
Garcia, Mariano, et al. "The simplest walking model: stability, complexity, and scaling." (1998): 281-288.
</p>


# Simple Walking Model
<br />

To begin my exploration of this kind of walking I used a simple model of a walking toy with 2 legs that was able to walk down a slope ramp without any actuation. This walker was name [Wobbly](https://www.thingiverse.com/thing:170932), and could be found on Thingiverse

<p align="center">
  <img src="http://krcarter.github.io/img/wobblyGif.gif" alt="passive Walking" width="400"/>
</p>


# My Gazebo Simulation
<br />

When it comes to robotics simulation software there is not that may readily available and have sophisticated enough physics engine to solve the constraints properly. So, I had a few options use a full body software like Webots or Gazebo or use Matlab and set up the simulation environment myself. I chose to use Gazebo since it easy to install in Linux and, I wouldn’t have to do the painstaking task of solving the hybrid transition states. 

<iframe width="800" height="533" src="https://www.youtube.com/embed/knAJdp4KJec" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<p align="center">
  <img src="http://krcarter.github.io/img/wobblyStates.png" alt="wobbly States" width="800"/>
</p>

<p align="center">
This figure is the robot states roll,pitch, and yaw.
</p>

<p align="center">
  <img src="http://krcarter.github.io/img/limitCycleFront.png" alt="limit Cycle Front" width="800"/>
</p>

<p align="center">
This figure is the state space plot of the resulting limit cycle.
</p>
