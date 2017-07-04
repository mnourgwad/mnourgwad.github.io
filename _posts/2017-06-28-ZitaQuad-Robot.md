---
layout: post
title: "ZitaQuad Robot: A Quadruped Walking Robot"
date: 2017-04-13
use_math: false
---

<p> This page gives a Summary of ZitaQuad Robot: A Quadruped Walking Robot Project</p>

## Report Summary
<p> 
In this report, we present the technical details of design, construction and control of a four-legged walking robot named ZitaQuad and the components that make up our final design are discussed. ZitaQuad robot is capable of basic mobility tasks such as walking forward, backward, and rotating. The legs are of a modular design that have three degrees of freedom each. This robot will serve as a platform onto which additional sensory components could be later added. Its implemented control software is programmed to perform increasingly complex tasks. Also, we describe the basic robot gaits of locomotion for efficient navigation. The robot motion is controlled through an android application over Bluetooth communication. The construction of the robot consists of mechanical structure, microcontroller board, and software program. 
</p>
<p> 
In the mechanical design, we use the SolidWorks program to design the robot mechanical parts. In resemblance to ant leg, the leg design consists of three parts coxa, femur, and tibia while the robot body is designed in rectangular shape. After the design of the parts is finalized, we used CNC machine to fabricate parts using acrylic sheet with thickness 2.5 mm. Some format conversions were made from SolidWorks part file type to dxf type suitable to CNC machine. To complete the construction of the robot, motor torques are calculate based on the mass and dimension of robot parts. Then the suitable motor sizes are selected and installed. We selected servo motors as they are internally position controlled and easily connected to the hardware.
The brain of our robot is contained in the main microcontroller board. Our main board is Arduino Mega. It is a microcontroller board based on the ATmega1280 with enough digital input/output pins, analog inputs, PWM outputs, and serial ports to accommodate needed connections to different robot components. Other sensors (ultrasonic to overcome obstacles) and components (Bluetooth board for communications) are also connected to the main board.
Finally, the high–level functionality and control of the robot are implemented in the robot software which consists of many modules. First module is implemented to provide the main robot specifications and dimensions such as: link lengths, minimum, and maximum joint angle limits. Other modules provide the walking algorithm of four legs. That is based on the robot forward and inverse kinematics. The whole robot kinematic equations are derived and implemented in the software. 
This project is foreseen to have very interesting extensions that can be added in the future. To name some, the simulation of the movement of insects as well as in the robot programming technology to overcome obstacles and also the ability to use Android software to control the robot remotely. In addition, more functions and components can be added in the future such as GPS, monitoring, and camera.
</p>
