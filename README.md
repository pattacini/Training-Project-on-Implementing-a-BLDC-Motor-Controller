# Training Project on Implementing a BLDC Motor Controller with Simscape Electrical and Stateflow

This repository consists of folders containing the MATLAB and Simulink files that are realized following the [How to Design Motor Controllers Using Simscape Electrical](https://www.mathworks.com/videos/series/how-to-design-motor-controllers-using-simscape-electrical.html) video tutorial series.

__Note that most of the MATLAB code is copied from [here](https://github.com/mathworks/Design-motor-controllers-with-Simscape-Electricalhttps://github.com/mathworks/Design-motor-controllers-with-Simscape-Electrical)__.


## ✅ Prerequisites
---

| Knowledge            | Level     |
| -------------        | ---------- |
| Control Theory       | ⭐⭐   
| Electronics Theroy   | ⭐⭐
| Simulink             | ⭐⭐⭐
| Stateflow            | ⭐⭐⭐
| Simscape             | ⭐⭐⭐
| Matlab               | ⭐


## 🎯 Goal
---

The purpose of this project is to implement a speed control system for a simple BLDC motor using the basic knowledge of Simulink, Simscape and Stateflow. 

| ![The system ](algorithm.png) |
| :---------------: |
| The block diagram of the BLCD control system (🔘 click on the image to enlarge) |


## Main Flow
---
This section shows the main steps I followed to achieve the goal.
  
1. [Simulink onramp](https://www.mathworks.com/learn/tutorials/simulink-onramp.html)
2. [Stateflow onramp](https://www.mathworks.com/learn/tutorials/stateflow-onramp.html)
3. BLDC Theory from different sources
    1. [An Introduction to Brushless DC Motors](https://www.youtube.com/watch?v=gNpoTPzEkco)
    2. [Brushless DC electric motor](https://en.wikipedia.org/wiki/Brushless_DC_electric_motor)
    3. [bldc-motor-control](https://www.mathworks.com/solutions/power-electronics-control/bldc-motor-control.html)
4. Simulink implementation simulating the Back-EMF Voltage of a BLDC Motor
5. Implementing a Three-Phase Inverter to drive the BLDC motor
6. Implementing the commutation logic in order control a BLDC motor at constant speed.
    1. Implementing the PID controller that lets us control the motor at different speeds and simulate motor response.
    2. Replace the commutation logic with a new one using Stateflow.
7. Trying to add a PWM Control with the aim to achieve a more realistic scenarious (⚠ Work in progress).

__Note__:
Each folder contains a README that shows the main work of the relative step.


## 👀 See also
---
Check out [this tech talk video series](https://www.mathworks.com/videos/series/brushless-dc-motors.html) to understand: 
  
- How brushless DC motors differ from brushed DC motors and how they work
- How BLDC motors can be controlled using six-step commutation (trapezoidal control)
- The different components of a BLDC motor control algorithm such as PWM control, commutation logic, three-phase inverter and sensor
