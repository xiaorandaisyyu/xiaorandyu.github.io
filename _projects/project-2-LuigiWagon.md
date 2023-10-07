---
title: "Luigi Wagon: an FPGA-based IoT System"
excerpt: "An IoT system that supports multiple player nodes to exchange information with a cloud server, in order to play a video game, Luigi Wagon (inspired by Mario Kart). <br/><img src='/images/500x300.png'>"
collection: projects
---
[GitHub Repo](http://xiaorandyu.github.io/)  [Report PDF](http://xiaorandyu.github.io/files/EEEBalanceBug.pdf)

## Overview
This project is part of my second year Information Processing coursework in which our group developed an IoT system that supports multiple player nodes to exchange information with a cloud server, in order to play a video game, Luigi Wagon (inspired by Mario Kart). The coursework was completed in groups of six, and our group received high appreciations on both the oral presentation and the writtern report (A+). 

## Project Outline
The project intended to make use of the knowledge acquired in various modules, such as Software Systems (networking, database), Signals & Systems, Instruction Architectures (Verilog, CPUs), and Discrete Maths (algorithms, complexity). 

Data was captured by the accelerometer on FPGA boards as user controller input. UART was utilised for 2-way communication between nodes and a host PC. UDP was chosen for communication between the host PC and the EC2 server. DynamoDB was used as a NoSQL database for storing player data. Later enhancements on user experience include the reduction of multiplayer latency and the FPGA input latency.

The game client was originally coded in Python with the PyGame library, then switched to Unity (C#) for a more entertaining 3D setting.

## Personal Contribution
I was the person behind the FPGA-side, being responsible for all setups (hardware & software) on FPGA, local processing of accelerometer data (in software), and establishment of 2-way communication between FPGA outputs and host through UART. 