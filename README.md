# Ultrasonic-Obstacle-Detection-QA
Arduino-based obstacle detection using an HC-SR04 ultrasonic sensor, LED indicators, and GitHub QA issue tracking.

# Ultrasonic Obstacle Detection System

## Project Overview
This embedded system uses an HC-SR04 ultrasonic sensor and an Arduino Uno to measure the distance of nearby objects and indicate obstacle status using red and green LEDs.

## Objectives
- Measure object distance using an ultrasonic sensor.
- Detect obstacles within a 10 cm threshold.
- Provide visual feedback using LEDs.
- Document QA findings and track improvements using GitHub Issues.

## Hardware Requirements
- Arduino Uno
- HC-SR04 ultrasonic sensor
- Red and green LEDs
- Two 220 Ω resistors
- Jumper wires and breadboard

## Pin Connections
| Component | Arduino Pin |
|---|---|
| TRIG | D9 |
| ECHO | D10 |
| Red LED | D6 |
| Green LED | D7 |

Connect the sensor VCC to 5V and GND to GND. Connect each LED through a current-limiting resistor, with its cathode connected to GND.

## Working Principle
The sensor measures the time taken by an ultrasonic pulse to return from an object. The Arduino calculates the distance and compares it with the configured threshold.

- Distance below 10 cm: Red LED ON.
- Distance equal to or above 10 cm: Green LED ON.
- Invalid sensor reading: Both LEDs OFF and an error message displayed.

## Software
- Arduino IDE
- Embedded C/C++ (Arduino framework)
- GitHub for version control and QA issue tracking

## Testing
The project includes sensor-timeout checks, distance-threshold test cases, LED indication checks, and documentation review. Record actual results and specify whether each test was performed using physical hardware, simulation, or code review.

## QA and Project Tracking
Potential issues and improvements are recorded in GitHub Issues. Code changes, comments, and issue status updates provide a record of the development process.
