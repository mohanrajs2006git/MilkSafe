# 🥛 MilkSafe - An IoT-Powered Milk Freshness Analyzer Using Sensors and Machine Learning

This repository presents the design and implementation of an IoT-powered Milk Spoilage Analyzer using smart sensors and a machine learning model. It enables real-time monitoring, predictive analytics, and early warnings to ensure milk safety, reduce wastage, and optimize the dairy supply chain.

## Contents

- [Introduction](#introduction)
- [Overview](#overview)
- [Goals and Objectives](#goals-and-objectives)
- [Target Audience](#target-audience)
- [Key Features](#key-features)
- [Technical Approach](#technical-approach)
- [Required Components and Bill of Materials](#required-components-and-bill-of-materials)
- [Block Diagram](#block-diagram)
- [Circuit Diagram](#circuit-diagram)
- [Pin Connections](#pin-connections)
- [Sensor Details](#sensor-details)
- [Working Code](#working-code)
- [Application Videos](#application-videos)
- [Final Product](#final-product)
- [Contributors](#contributors)
- [Acknowledgements](#acknowledgements)
- [Contact Information](#contact-information)

## Introduction

Milk is one of the most consumed dairy products worldwide, but it is also highly 
perishable. Every day, millions of liters of milk are wasted due to spoilage caused by 
improper storage, transportation delays, and lack of proper monitoring methods. In many 
rural collection centers, milk is tested only for fat and SNF (Solid-Not-Fat), without any 
microbial or freshness assessment, leading to spoilage before reaching processing units. 
This results in economic loss and health risks due to accidental consumption of spoiled 
milk. 
To address this issue, our project proposes a smart milk spoilage detection system that can 
monitor the freshness of milk in real-time. The system integrates multiple sensors—pH 
sensor, temperature sensor, gas sensor, and turbidity sensor—to detect early signs of 
spoilage. These sensors are connected to the ESP32 microcontroller, which collects the 
data, processes it, and sends alerts when milk quality falls below safe levels. 
The ESP32 enables wireless communication through Wi-Fi or Bluetooth, allowing the 
system to transmit real-time data to a cloud platform or mobile app for remote monitoring. 
This provides users—farmers, dairy transporters, and processing centers—with up-to-date 
information on milk conditions during storage and transportation. 
By implementing this system, the project aims to improve milk safety, reduce post-harvest 
losses, and enhance the efficiency of the dairy supply chain, especially in rural areas. It 
offers a cost-effective, portable, and easy-to-use solution to ensure that only fresh and safe 
milk reaches consumers, supporting both public health and the dairy industry. 
## Overview

The MilkSafe system uses:

- ESP32 microcontroller
- E201-BNC pH sensor
- MQ-135 gas sensor
- DS18B20 temperature sensor

Data is collected and transmitted for analysis. A trained ML model predicts spoilage time, and results are shown on a user-friendly dashboard.

## Goals and Objectives
The main objective of this project is to develop a real-time milk spoilage detection system 
using smart sensors and a microcontroller to ensure milk quality during storage and 
transportation. The system aims to: 
1. To monitor key freshness parameters such as pH, temperature, turbidity, and gas 
levels in milk. 
2. To detect early signs of spoilage using sensor data, helping prevent health risks and 
3 
reduce milk wastage. 
3. To enable real-time alerts and remote monitoring of milk quality through ESP32
based wireless communication. 
4. To provide rural milk collection centers with an affordable and easy-to-use spoilage 
detection system.

## Target Audience

- Dairy farmers
- Milk collection centers
- Dairy processing units
- Rural cooperatives
- Researchers and innovators in food safety

## Key Features

Integration of several sensors (turbidity, pH, temperature, and gas) to track key 
factors influencing milk freshness 
 Utilization of the ESP32 microcontroller for data collection, processing, and wireless 
connectivity 
 Real-time alerts via IoT to inform users of any fall in milk quality 
 Remote monitoring ability through mobile or web portals, improving decision
making and prevention measures 
 Implementation in rural milk collection centers, transport vehicles, cold storage 
facilities, and dairy processing plants 
 Decrease in wastage of milk and financial loss by determining spoilage prior to 
processing units 
 Guaranteeing safety for the consumer by stopping supply of rotten milk into the 
market 
 The system is designed to be cost-effective, scalable, and easy to deploy, making it 
suitable for both small-scale and large-scale dairy operations. In the future, it can be 
extended to include cloud data storage, data analytics, and machine learning 
algorithms for predictive spoilage detection

## Technical Approach

- **Hardware:** ESP32, MQ-135, DS18B20, E201-BNC  
- **Software:** Arduino IDE for ESP32, Python for data processing  
- **ML Model:** Random Forest Regressor  
- **Output Interface:** Web dashboard (Python Matplotlib + Pandas)

## Required Components and Bill of Materials

| Component           | Quantity | Cost (INR) |
|---------------------|----------|------------|
| ESP32               | 1        | ₹350       |
| E201-BNC pH Sensor  | 1        | ₹1700      |
| MQ-135 Gas Sensor   | 1        | ₹200       |
| DS18B20 Temp Sensor | 1        | ₹100       |
| Jumper Wires        | 1 set    | ₹50        |
| Breadboard          | 1        | ₹80        |
| Battery / USB       | 1        | ₹30        |
| **Total**           | –        | **₹2,510** |

## Block Diagram

![Block Diagram](images/Blockdiagram.jpg)


## Pin Connections

| Sensor   | ESP32 Pin   |
|----------|-------------|
| MQ-135   | GPIO36 (A0) |
| DS18B20  | GPIO15      |
| E201-BNC | GPIO39 (A3) |

## Sensor Details

- **pH Sensor:** Detects increasing acidity (spoilage indicator)  
- **Gas Sensor:** Detects ammonia/H₂S from microbial activity  
- **Temp Sensor:** Detects cold chain breach  

## Application Videos

- 📽 Spoilage Detection & Alert  
- 📽 Dashboard Visuals of Sensor Readings  
- 📽 Sample Classification and Spoilage Countdown  

## Final Product

A compact IoT system with a connected sensor network, dashboard visualization, and ML-powered prediction, deployable in rural and commercial environments.

## Contributors

- Mohan Raj S  
- Likhit S  
- Manishankar M  
- Naveensurya V  

## Acknowledgements

- Dr. S. Ramkumar, Associate Professor, ECE, Sri Eshwar College of Engineering  

## Contact Information

- Mohan Raj S – [mohanrajs.ec2023@gmail.com](mailto:mohanrajs.ec2023@gmail.com)  
- Institution: Sri Eshwar College of Engineering  
- Duration: Jan – May 2025
