# Automated Milk Quality Analysis System  
### (Microbial Load Detection + Water Content Measurement)

## Overview
This project presents an integrated, automated  milk quality analysis system that combines:
1. Impedance-based microbial load detection
2. Automatic milk-to-curd conversion with whey (water) measurement

The system is designed to provide rapid, accurate, and hygienic assessment of milk quality without relying on conventional laboratory tests.

---

## Motivation
Traditional milk quality tests such as MBRT, lactometer testing, and manual curd formation:
- Are time-consuming
- Depend heavily on human judgment
- Require chemicals and laboratory setup
- Are unsuitable for on-site decision making

This project addresses these issues by automating both **microbial freshness detection** and **water/adulteration analysis** in a single system.

---

## System Architecture
The project consists of two sequential modules:

### Module 1: Microbial Load Detection (Impedance Sensing)
- Rapid screening of milk freshness
- Non-destructive and reagent-free
- Provides quality classification

### Module 2: Water Content Detection (Curd–Whey Method)
- Controlled heating and citric acid dosing
- Automated whey separation
- Quantitative water percentage calculation

---

## Methodology

### Step 1: Impedance-Based Microbial Analysis
1. Milk sample is placed in the test chamber
2. Stainless steel electrodes are immersed
3. Low-amplitude AC signal is applied
4. Electrical impedance is measured
5. Microcontroller classifies milk as:
   - Fresh
   - Moderately contaminated
   - Spoiled

### Step 2: Automated Milk-to-Curd & Whey Measurement
1. Milk is heated automatically up to 70 °C
2. Heater switches OFF at set temperature
3. Citric acid is added using a peristaltic pump
4. Curd formation occurs
5. Whey is separated using filtration
6. Whey weight is measured using a load cell
7. Water percentage is calculated

---

## Water Percentage Formula
Water Percentage = (Volume of Whey / Volume of Milk) × 100

---

## Hardware Components
- Microcontroller (Arduino UNO / ESP32)
- AD5933 Impedance Analyzer
- Stainless Steel Food-Grade Electrodes
- Temperature Sensor (DS18B20 / LM35)
- Electric Heater + Relay Module
- Peristaltic Pump
- Load Cell with HX711
- Food-Grade Filter Assembly
- LCD / OLED Display
- Rechargeable Power Supply
- servo motor

---

## Key Features
- Dual-method milk quality analysis in one system
- Fast microbial freshness detection
- Accurate water/adulteration measurement
- Fully automated operation
- Improved hygiene and repeatability
- Suitable for on-site testing

---

## Applications
- Milk collection centers
- Dairy farms and cooperatives
- Quality control laboratories
- Food technology education
- Embedded systems and EDP projects

---

## Limitations
- Requires calibration for different milk types
- Impedance method gives estimated microbial load, not exact CFU
- Sensor accuracy depends on temperature stability

---

## Future Scope
- IoT-based data logging and cloud monitoring
- Mobile app integration
- Machine learning for microbial prediction
- Industrial-scale deployment
- Automated cleaning (CIP) system

---

## Conclusion
This integrated project demonstrates how sensor-based automation can significantly improve milk quality assessment by combining rapid microbial screening with accurate water content analysis, making it a practical and scalable solution for modern dairy quality control.
