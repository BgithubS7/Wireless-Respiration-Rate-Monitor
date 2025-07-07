# Wireless Respiration Rate Monitor

A low-cost, very portable, wireless system that monitors human respiration rate using a chest-mounted sensor and transmits data via Bluetooth to a mobile or PC dashboard.

## 🛠️ Features
- Sensor for the heart rate movements 
- ESP32 for Bluetooth and processing
- Real-time plotting on phone or PC
- Battery-powered and wearable
- Accurate breath detection via signal filtering
- Analog and digital circuit
- C++ and python
- rf

## 📷 Preview!
- This figure below shows the entire design flow chart and my thought process of what I would like the device to look like and do.
- In the HIGH LEVEL DESIGN: https://github.com/BgithubS7/Wireless-Respiration-Rate-Monitor/blob/main/High%20Level%20Design
- I have clearly explained the function of each block, why I decided to choose such component given the contraints that I have to work with. 

![Image](https://github.com/user-attachments/assets/9e403b4c-355f-491b-a136-9fbd4f3e57dd)
For explanation, please visit the schematic document at: https://github.com/BgithubS7/Wireless-Respiration-Rate-Monitor/blob/main/SCHEMATIC%20DOCUMENT





## 📂 Project Structure
#  `/Hardware Design/` – Schematics and PCB files
- After coming up with the high level architecture for the design, I went on to drawing the schematic and looking for each component that is most compatible with my desing, especially since I consider power and sensitivity to be of great factor in the sleep mode and regular mode and when getting the respiration reading.
- The `/Schematic/` folder contains all Altium design files, schematics, and layout resources for the project.

  ### 📷 Schematics
  #### 🔌 Sensor Schematic:
  ![Image](https://github.com/user-attachments/assets/de3a001b-33fb-4d36-aaef-08a6199daafd)

  ---
  
  #### 🎯 Connectivity Schematic
  
![Image](https://github.com/user-attachments/assets/a6e00782-9c33-4600-a9ff-f67ca3c78cee)


### Design Philosophy

The architecture reflects a careful balance of:

- **Power Efficiency**  
  Optimized voltage regulation using DC-DC converters and low-voltage logic levels to minimize power consumption and heat generation.

- **Signal Integrity**  
  Proper I²C pull-up configuration, separation of power domains, and noise-aware routing practices ensure reliable high-speed communication.

- **Component Protection**  
  Load switches isolate sensitive circuitry and prevent unintended current surges, while power rails are regulated within tight tolerances.

- **System-Level Control**  
  Firmware-controlled power gating via load switches allows dynamic control of subsystem power, enabling smarter power budgeting and modularity.

- For furtehr explanation visit: https://github.com/BgithubS7/Wireless-Respiration-Rate-Monitor/edit/main/SCHEMATIC%20DOCUMENT
  
- `/firmware/` – Embedded C / C++ code for ESP32
- `/mobile-app/` – Optional dashboard (e.g., Flutter)-python GUI
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
