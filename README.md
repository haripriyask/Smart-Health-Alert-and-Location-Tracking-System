# Smart Health Alert and Location Tracking System
An ESP32-based IoT system for real-time monitoring of heart rate, motion, and GPS location. Sensor data is uploaded to ThingSpeak for visualization, and abnormal conditions trigger instant mobile alerts using IFTTT for emergency response.

## Description
This project is an IoT-based real-time health and location monitoring system using ESP32. It monitors heart rate, body movement, and GPS location continuously.If any abnormal condition like low heart rate, no movement, or GPS loss is detected, the system sends an emergency alert to the user through mobile notification.

## Objective
- Monitor heart rate in real time
- Track location using GPS
- Detect body movement or fall
- Send emergency alerts

## Components Used
- ESP32
- MAX30102 (Heart Rate Sensor)
- MPU6050 (Motion Sensor)
- GPS Module (Neo-6M)
- Wi-Fi

## Working
1. Sensors collect health and movement data
2. ESP32 processes the data
3. Data is sent to ThingSpeak cloud
4. MATLAB checks abnormal conditions
5. IFTTT sends alert to mobile

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
