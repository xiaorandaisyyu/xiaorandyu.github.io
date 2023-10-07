---
title: "EEEBalanceBug: Second Year Group Design Project"
excerpt: "An autonomous 2-wheel balancing rover that is capable of navigating through a maze and creating a map of it. <br/><img src='/images/500x300.png'>"
collection: projects
---
[GitHub Repo](http://xiaorandyu.github.io/)  [Report PDF](http://xiaorandyu.github.io/files/EEEBalanceBug.pdf)

## Overview
In my second year final project (Computer Engineering Design Project), I worked closely with another 3 EIE students and 2 EEE students to design and build an autonomous 2-wheel balancing rover that is capable of navigating through a maze and creating a map of it. Our project was evaluated in various perspectives (automaticity, robustness, usability, testability, maintainability, scalability, etc.), after which, our group received an overall mark of 72.61%.

## Project Outline
In addition to a maze-solving rover, the project embodies several other components as well. 

Illuminated beacons powered by an emulated photovoltaic panel were placed around the edge of the maze and were used for position triangulation during mapping. The rover was mounted with a camera on an FPGA to capture, filter, and analyse the maze’s environment. It was also loaded with a ESP32 microcontroller for processing of sensor data, driving of the motors, impletation of maze-exploring algorithm, and data communications with server. The vectorised map constructed using the MySQL database on the server could be further investigated to determine the shortest path.

The maze-exploring algorithm itself, blended movement commands together with a process stack, which implements a state machine that follows the predetermined depth-first principle. The previously explored paths were gathered and linked as a node graph and stored in a hash-table. 

(Please refer to “Abstract” section in the report for more details.)

## Personal Contribution
I mainly focused on the FPGA-related part of work, implemented various image processing and filtering programs to extract useful information about the maze using the video input from D8M camera, and established communications between FPGA and ESP32 with different methods. I also contributed to the development and testing of the maze-exploring algorithm and chassis design.