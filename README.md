# Edge_AI-Human-Animal-Prediction
This project implements an Edge AI system using ESP32‑CAM to detect whether the captured image contains a human or an animal. The system uses a machine learning model trained with Edge Impulse and runs inference directly on the ESP32 device.

# Human vs Animal Detection using ESP32-CAM and Edge Impulse

This project demonstrates an **Edge AI application** where an ESP32-CAM device captures an image and classifies whether the object is a **Human** or an **Animal** using a machine learning model trained with **Edge Impulse**.

The entire inference runs directly on the **ESP32 microcontroller**, making it a lightweight and real-time Edge AI system.

---

## Project Overview

Edge AI allows machine learning models to run directly on embedded hardware without relying on cloud computation.  

In this project:

1. Images were collected and uploaded to **Edge Impulse Studio**
2. A classification model was trained
3. The model was deployed as an **Arduino library**
4. The ESP32-CAM captures an image and runs inference locally

---

## Hardware Used

- ESP32-CAM module
- ESP-CAM-MB programmer
- USB cable
- Laptop

---

## Software & Tools

- Arduino IDE
- Edge Impulse Web Studio
- ESP32 Arduino Core
- Edge Impulse SDK

---

## Machine Learning Model

Classes used:
  1.Human
  2.Animal


Training pipeline:

    Image Input
        ↓
    Image Processing
        ↓
    Classification Neural Network
Image size used: **96x96**
Resize mode: Squash

---

## System Architecture

<img width="1000" height="421" alt="image" src="https://github.com/user-attachments/assets/743456ce-15d6-403b-af73-596bd6454ccd" />


---

## Installation & Setup

### 1 Install Arduino IDE
Download:
https://www.arduino.cc/en/software

### 2 Install ESP32 Board

Add this URL in Arduino Preferences:
https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json

Then install **ESP32 boards** from Board Manager.

---

### 3 Install Edge Impulse Library

Download the Arduino library from Edge Impulse deployment section and install:
Sketch → Include Library → Add .ZIP Library

---

### 4 Select Board Settings
Board: AI Thinker ESP32-CAM
PSRAM: Enabled
Partition Scheme: Huge APP
Upload Speed: 115200

---

### 5 Upload Code

Upload the Arduino sketch from:
arduino_code/esp32_edge_ai.ino

---

## Output

Serial Monitor Output:

1. output for animal image <img width="702" height="422" alt="image" src="https://github.com/user-attachments/assets/e319965b-78fd-4ca5-9e40-596fca8122bc" />

2. output for human image <img width="632" height="422" alt="image" src="https://github.com/user-attachments/assets/8615433a-beb8-408e-be02-06b576abfcc4" />
 

---

## Applications

- Smart security cameras
- Wildlife monitoring
- Farm animal monitoring
- Edge AI research projects
- Smart IoT devices

---

## Future Improvements

- Real-time camera streaming
- Bounding box detection
- Telegram alerts for detection
- Higher accuracy models

---

## Author

**Dhanush Babu Ravinuthala**

Master's Student – Data Science  
Germany

---

## Acknowledgements

- Edge Impulse
- Espressif ESP32
- Arduino Community
- Hochschule Fulda
- Prof. Ivan Jursic
