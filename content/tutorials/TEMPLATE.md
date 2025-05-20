---
title: Calculating Distance using ESP32
date: 2025-05-019
authors:
  - name: Ace Chikazawa
---

[![HC-SR04](https://techknowlab.com/wp-content/uploads/2025/02/HC-SR04.jpg)]

## Introduction

This tutorial introduces students on how to use ultrasonic distance sensors with an ESP32 and using those readings to generate a PWM signal to then control the output of an ESP32. From this tutorial students will learn to calibrate sensors and get accurate real-world measurements to drive an output device.

The motivation behind this tutorial is to introduce students to various different input and output sustems that can be applied to other real world applications. 

### Learning Objectives

+ Bread boarding
+ PWM control
+ Using an ultrasonic sensor
+ Sensor input calibration

### Background Information

A proximity sensor is used to measure the distance between the sensor and an obstacle by sending pulsing high frequency noises and calculating the time between the pulse and the echo. We are using an HC-SR04 due to its afforable and ease of set up. Other distance sensors exist but they are much more expensive or are much harder to setup. The drawback of these ultra sonic sensors are their difficulty gathering accurate data when used against sound absorbing material. 

PWM signals are high frequency pulses as well that determine the voltage output to a device. A PWM signal is a digital signal that uses the duty cycle of high and low signals to essentially create an analog signal from digital high and low signals. 


## Getting Started

For any software prerequisites, write a simple excerpt on each
technology the participant will be expecting to download and install.
Aim to demystify the technologies being used and explain any design
decisions that were taken. Walk through the installation processes
in detail. Be aware of any operating system differences.
For hardware prerequisites, list all the necessary components that
the participant will receive. A table showing component names and
quantities should suffice. Link any reference sheets or guides that
the participant may need.
The following are stylistic examples of possible prerequisites,
customize these for each workshop.

### Required Downloads and Installations

List any required downloads and installations here.
Make sure to include tutorials on how to install them.
You can either make your own tutorials or include a link to them.

### Required Components

List your required hardware components and the quantities here.

| Component Name  | Quanitity |
| ESP32 dev board |     1     |
| HC-SR04 Sensor  |     1     |
| Piezzo Buzzer   |     1     |
| Bread Board     |     1     |
| Jumper Cables   |     1     |
| USB typeC cable |     1     |


### Required Tools and Equipment

- Computer with USB port
- Arduino IDE
- Internet Access

## Part 01: Name

### Introduction

Briefly introduce what  you are teaching in this section.

### Objective

- List the learning objectives of this section

### Background Information

Give a brief explanation of the technical skills learned/needed
in this challenge. There is no need to go into detail as a
separation document should be prepared to explain more in depth
about the technical skills

### Components

- List the components needed in this challenge

### Instructional

Step 1: Setting up project space
  Download all required software for this project
  - Assemble ESP32 board if not already assembled
  - Download Arduino IDE through this link (insert link later)
  - Collect all needed materials (listed in required components section above)
  - 

Step 2: Connect HC-SR04 to ESP32
  Connect the following pins on the ultrasonic sensor to the pins on the ESP32
  + VCC -> 5V
  + GND -> GND
  + Trig -> GPIO of your choosing
  + Echo -> GPIO of your choosing

Step 3: Setting up in Arduino IDE
  Input code to have initial setup of ultrasonic sensors
  #define TRIG_PIN (previously chosen value)
  #define ECHO_PIN (previously chosen value)

  void_setup() {
    Serial.begin(115200);
    pinMode(TRIG_PIN, OUTPUT);
    pinMode(ECHO_PIN, INPUT);
  }

  
 

## Example

### Introduction

Introduce the example that you are showing here.

### Example

Present the example here. Include visuals to help better understanding

### Analysis

Explain how the example used your tutorial topic. Give in-depth analysis of each part and show your understanding of the tutorial topic

## Additional Resources

### Useful links

List any sources you used, documentation, helpful examples, similar projects etc.
