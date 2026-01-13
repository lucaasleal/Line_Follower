# Line Follower Robot with PID Control

This project implements a **line follower robot** using an array of **QTR reflectance sensors** and a **PID-based control strategy** to keep the robot centered on a line. The system is designed to run on an Arduino-compatible microcontroller and controls two DC motors via PWM.

## 🚗 Overview

The robot continuously reads data from 8 infrared sensors to detect the position of a line on the ground. Based on this information, a PID controller computes a correction value that adjusts the speed of each motor, allowing smooth and stable line tracking.

## ⚙️ Main Features

- 8-channel QTR reflectance sensor array  
- Automatic sensor calibration  
- PID control (Proportional + Integral)  
- Differential motor speed control using PWM  
- Real-time sensor monitoring via Serial output  

## 🧠 Control Strategy

- The sensor array estimates the line position relative to the robot center  
- A normalized error value is computed in the range **(-1, 1)**  
- The PID controller generates a correction signal  
- Motor speeds are adjusted to steer the robot back to the line  

## 🛠️ Technologies Used

- Arduino (C/C++)
- QTRSensors library
- DC motors with PWM control
- Infrared reflectance sensors

## 📌 Notes

- Sensor calibration is required at startup  
- PID constants can be tuned for different tracks and speeds  
- Designed for educational and experimental robotics projects  

## 📜 License

This project is intended for academic and learning purposes.
