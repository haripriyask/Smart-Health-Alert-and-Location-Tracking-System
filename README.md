# Smart Health Alert and Location Tracking System
An ESP32-based IoT system for real-time monitoring of heart rate, motion, and GPS location. Sensor data is uploaded to ThingSpeak for visualization, and abnormal conditions trigger instant mobile alerts using IFTTT for emergency response.

## Description
The proposed system uses ESP32 as the central microcontroller. It collects data from the GPS module to determine location (latitude, longitude, speed), from the MAX30102 sensor to measure heart rate, and from the MPU6050 to detect movement or potential falls. This data is transmitted to ThingSpeak using HTTP. MATLAB code on ThingSpeak analyzes the data to detect emergency conditions. If such a condition is identified (e.g., heart rate is zero, or GPS is inactive), it triggers an IFTTT webhook which sends a mobile notification to the caregiver.

## Objective
The objective of this project is to develop a microcontroller-based wearable system using ESP32 that can:
• Monitor GPS coordinates to track location
• Measure pulse and detect abnormal heart rates
• Detect sudden or complete lack of motion
• Transmit all parameters to a cloud server (ThingSpeak)
Alert designated individuals via mobile notifications using IFTTT in
emergency cases.

## Components Used

### Software:
- Arduino IDE: For firmware programming
- ThingSpeak: Cloud platform for visualization and processing
- MATLAB: Script execution for automated alert conditions
- IFTTT: Mobile notification trigger service

### Hardware:
- ESP32: Powerful Wi-Fi enabled microcontroller
- Neo6M GPS: For real-time location tracking
- MAX30102: Pulse oximeter and heart rate sensor
- MPU6050: Detects motion, orientation, falls

### Communication Interface:
- I2C: Used by MAX30102 and MPU6050
- UART: Used by GPS module
- Wi-Fi: ESP32 communicates with ThingSpeak and IFTTT via HTTP

## Working
1. Sensors collect health and movement data
2. ESP32 processes the data
3. Data is sent to ThingSpeak cloud
4. MATLAB checks abnormal conditions
5. IFTTT sends alert to mobile

## United Nations SDG(s) Mapped to the Project

This project aligns with multiple Sustainable Development Goals (SDGs):

- **GOAL 3 – Good Health and Well-Being:** By enabling real-time monitoring and alerts, this project enhances preventive care and emergency response.
- **GOAL 9 – Industry, Innovation and Infrastructure:** It demonstrates innovative use of IoT and communication systems to build a cost-effective healthcare tool.
- **GOAL 11 – Sustainable Cities and Communities:** Promotes safe and resilient health support infrastructure for elderly and vulnerable populations.

## Features
- Real-time monitoring
- Emergency alert system
- Cloud data visualization
- Remote access

## Applications
- Elderly health monitoring
- Patient safety system
- Child tracking

## CONCLUSION
The system successfully demonstrates a smart wearable health tracker with cloud integration and real-time alerting. Using ESP32 and ThingSpeak, the patient’s condition and location can be monitored remotely. IFTTT ensures that emergency alerts reach caregivers instantly, potentially saving lives in critical situations. The combination of GPS, heart monitoring, and motion tracking makes the solution robust, affordable, and adaptable for personal and medical use.
