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

Milk spoilage leads to massive wastage and potential health risks due to microbial contamination, especially in rural collection centers lacking real-time monitoring tools. This project presents **MilkSafe**—a smart, real-time monitoring system using IoT and machine learning to track freshness and alert before spoilage.

## Overview

The MilkSafe system uses:

- ESP32 microcontroller
- E201-BNC pH sensor
- MQ-135 gas sensor
- DS18B20 temperature sensor

Data is collected and transmitted for analysis. A trained ML model predicts spoilage time, and results are shown on a user-friendly dashboard.

## Goals and Objectives

🎯 Monitor gas levels, pH, and temperature in real-time  
🎯 Predict spoilage using machine learning  
🎯 Provide freshness classification: Fresh / Warning / Spoiled  
🎯 Alert users early to avoid health hazards and wastage  
🎯 Reduce post-harvest dairy loss through smart intervention

## Target Audience

- Dairy farmers
- Milk collection centers
- Dairy processing units
- Rural cooperatives
- Researchers and innovators in food safety

## Key Features

📌 Real-time sensor monitoring via ESP32  
📌 Freshness prediction using Random Forest algorithm  
📌 Visual dashboard displaying sensor trends  
📌 Classifies samples as Fresh, Warning, or Spoiled  
📌 Low-cost, portable, and easy-to-use hardware system

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

```
[pH Sensor] →  
[Gas Sensor] →  [ESP32] → [ML Model] → [Dashboard]  
[Temp Sensor] →
```

## Circuit Diagram

*To be uploaded as image or Fritzing diagram*

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

## Working Code

- Arduino script for sensor reading and serial data transmission  
- Python script for dashboard display and ML prediction  

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
