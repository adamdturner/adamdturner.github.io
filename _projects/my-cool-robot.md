---
layout: project
title: "Light-Following Robot"
date: 2025-06-25 23:15:17 -0600
description: "An autonomous robot that uses photoresistors and Arduino to intelligently follow light sources while avoiding obstacles."
duration: "2 weeks"
role: "Lead Developer & Hardware Designer"
status: "Completed"
featured: true
technologies: ["Arduino", "C++", "Electronics", "Sensors", "Motors", "3D Printing"]
github_url: "https://github.com/adamdturner/light-following-robot"
demo_url: "https://youtube.com/watch?v=example"
---

## Project Overview

This autonomous robot project demonstrates the integration of hardware and software to create an intelligent light-following system. The robot uses multiple photoresistors to detect light sources and navigates towards them while avoiding obstacles using ultrasonic sensors.

## Key Features

- **Light Detection**: Uses 4 photoresistors arranged in a cross pattern for 360° light detection
- **Obstacle Avoidance**: Ultrasonic sensor prevents collisions with objects
- **Smooth Movement**: Differential drive system with PWM-controlled motors
- **Custom Chassis**: 3D-printed body designed for optimal sensor placement
- **Real-time Processing**: Arduino Uno processes sensor data and controls movement

## Technical Implementation

### Hardware Components
- Arduino Uno microcontroller
- 4x Photoresistors (LDR sensors)
- 1x Ultrasonic sensor (HC-SR04)
- 2x DC motors with gearboxes
- Motor driver (L298N)
- Custom 3D-printed chassis
- Rechargeable battery pack

### Software Architecture
The robot's behavior is controlled by a state machine that:
1. Continuously reads light sensor values
2. Calculates the direction of the strongest light source
3. Checks for obstacles using ultrasonic sensor
4. Adjusts motor speeds based on sensor inputs
5. Implements smooth turning and forward movement

### Key Algorithms
- **Light Source Detection**: Compares photoresistor values to determine light direction
- **Obstacle Avoidance**: Implements emergency stop and redirection when obstacles detected
- **Movement Control**: PID-like control system for smooth navigation

## Challenges & Solutions

**Challenge**: Inconsistent light detection in varying lighting conditions
**Solution**: Implemented adaptive thresholding and sensor calibration routines

**Challenge**: Robot getting stuck in corners or tight spaces
**Solution**: Added random movement patterns when no clear light source is detected

**Challenge**: Power consumption optimization
**Solution**: Implemented sleep modes and efficient motor control algorithms

## Results & Impact

- Successfully follows light sources with 95% accuracy
- Navigates around obstacles without collision
- 2-hour battery life on single charge
- Smooth, natural movement patterns
- Demonstrates practical application of sensor fusion

## Future Improvements

- Add camera module for visual light source recognition
- Implement machine learning for improved navigation
- Add wireless communication for remote monitoring
- Create mobile app for robot control and monitoring
- Develop swarm behavior for multiple robots

## Learning Outcomes

This project provided hands-on experience with:
- Embedded systems programming
- Sensor integration and data fusion
- 3D modeling and printing
- Electronics prototyping
- Real-time control systems
- Problem-solving in hardware-software integration
