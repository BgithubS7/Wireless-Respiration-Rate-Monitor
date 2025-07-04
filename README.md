# Wireless Respiration Rate Monitor

A low-cost, very portable, wireless system that monitors human respiration rate using a chest-mounted sensor and transmits data via Bluetooth to a mobile or PC dashboard.

## 🛠️ Features
- Sensor for the heart rate movements 
- ESP32 for Bluetooth and processing
- Real-time plotting on phone or PC
- Battery-powered and wearable
- Accurate breath detection via signal filtering

## 📷 Preview!
- This figure below shows the entire design flow chart and my thought process of what I would like the device to look like and do.
- In the HIGH LEVEL DESIGN: https://github.com/BgithubS7/Wireless-Respiration-Rate-Monitor/blob/main/High%20Level%20Design
- I have clearly explained the function of each block, why I decided to choose such component given the contraints that I have to work with. 

![Image](https://github.com/user-attachments/assets/9e403b4c-355f-491b-a136-9fbd4f3e57dd)




## 📂 Project Structure
- `/hardware/` – Schematics and PCB files
- `/firmware/` – Embedded C / C++ code for ESP32
- `/mobile-app/` – Optional dashboard (e.g., Flutter)
- `/data/` – Sample logs and signal traces

## ⚙️ Tech Stack
- ESP32 (or Arduino Nano 33 BLE)
- BLE (Bluetooth Low Energy)
- Python or Android app for visualization
- MATLAB or Python for signal processing (optional)

## 📄 License
MIT License 

## 🙋‍♂️ Author
Bright Sona (https://github.com/BgithubS7)
