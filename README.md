# Classroom CO₂ Monitor


A compact air quality monitor for classrooms, built with an ESP32, a Sensirion SCD41 CO₂ sensor, and a MAX7219 LED matrix display.  
It measures **CO₂ concentration**, **temperature**, and **humidity**, displaying values locally and sending data to ThingSpeak and Home Assistant via ESPHome.

---

Overview

This project was created as part of a research project on indoor air quality in classrooms.  
It aims to provide a low-cost, open-source tool to visualize CO₂ levels and encourage better ventilation.

---

Components

- ESP32 DevKit — main microcontroller (Wi-Fi enabled)
- SCD41 CO₂ Sensor (Sensirion)
  - Range: 400–5000 ppm
  - Accuracy: ±(40 ppm + 5 %)
  - Integrated temperature and humidity sensing
- MAX7219 LED Matrix Display
  - 8×8×4 module (controlled via SPI)
  - Brightness adjustable via software
- 5 V USB Power Supply
- 3D-Printed Enclosure 

---

Wiring Connections

| Component | ESP32 Pin | Description |
|------------|------------|-------------|
| SCD41 SDA  | GPIO21 | I²C data line |
| SCD41 SCL  | GPIO22 | I²C clock line |
| MAX7219 DIN | GPIO23 | SPI data |
| MAX7219 CLK | GPIO18 | SPI clock |
| MAX7219 CS  | GPIO5  | Chip Select |
| VCC / GND   | 5 V / GND | Power supply |


