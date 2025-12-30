# 🏠 Voice-Controlled Home Automation

<p align="center">
  <img src="docs/images/home_automation_overview.jpg" width="750" alt="Home Automation Overview">
</p>

A **home automation system** designed for **voice control via Google Home**, manual switch control, and real-time monitoring of **temperature, humidity, and light intensity**.  
The system integrates **IoT cloud services**, **OLED display feedback**, and **relay-based appliance control**, demonstrating smart home automation principles.

---

## 📸 DEMONSTRATION

<p align="center">
  <img src="docs/images/demo.gif" width="650" alt="Home Automation Demo">
</p>

---

# 📌 PROJECT CONTEXT

- **Academic Level:** Semester 3 – ECE  
- **Project Type:** Individual/Team embedded IoT project  
- **Focus Areas:**
  - Embedded systems & IoT
  - Home automation & smart devices
  - Cloud integration & Google Home voice control
  - Sensor fusion and data visualization
  - Hardware–software co-design

The goal is to **control appliances intelligently**, monitor environmental conditions, and showcase **secure IoT integration**.

---

# 📐 SYSTEM OVERVIEW

<p align="center">
  <img src="docs/images/system_block_diagram.png" width="650" alt="System Block Diagram">
</p>

The system consists of **four major subsystems**:

1. **Microcontroller** – central processing unit  
2. **Relay-Controlled Appliances** – devices toggled via voice or manual switch  
3. **Sensors & Display** – DHT11, LDR, OLED display  
4. **Cloud & Voice Interface** – Arduino IoT Cloud and Google Home integration  

---

# ⚙️ HARDWARE ARCHITECTURE

<p align="center">
  <img src="docs/images/hardware_setup.jpg" width="650" alt="Hardware Setup">
</p>

### 🔌 PIN CONFIGURATION

| Component | Pin |
|-----------|-----|
| DHT11 Sensor | GPIO 4 |
| Relay Module | GPIO 25 |
| Push Button Switch | GPIO 13 |
| LDR (Photoresistor) | GPIO 34 |
| OLED Display (I2C) | SDA → 21, SCL → 22 |
| Wi-Fi LED (Status) | GPIO 2 |

---

# ⚡ POWER SYSTEM

- Microcontroller powered via **regulated 5 V supply**  
- Relays powered by **external 5 V/12 V** depending on appliance  
- Shared ground ensures **stable operation and sensor reading integrity**  

---

# 🧠 CONTROL & FIRMWARE ARCHITECTURE

Firmware modules:

- **Cloud Communication** – Arduino IoT Cloud integration  
- **Voice Control Handling** – Google Home triggers relay state via cloud  
- **Manual Switch Handling** – push button overrides relay state  
- **Sensor Acquisition** – temperature, humidity, light intensity  
- **OLED Display** – cycles between sensor readings every 5 seconds  
- **Task Scheduling** – ensures smooth operation and real-time updates  

---

# 🤖 VOICE & MANUAL CONTROL

## 🗣️ VOICE CONTROL

- Controlled via **Google Home** linked to Arduino IoT Cloud  
- Example command: *“Hey Google, turn on the living room light”*  
- Updates cloud properties, reflected immediately on the microcontroller and OLED  

## 🔘 MANUAL SWITCH CONTROL

- Physical switch toggles relay on/off  
- Cloud and OLED states updated synchronously  

---

# 🖥 OLED DISPLAY FEEDBACK

<p align="center">
  <img src="docs/images/oled_display.jpg" width="450" alt="OLED Display">
</p>

- **Temperature:** °C  
- **Humidity:** %  
- **Light Intensity:** %  
- Cycles display automatically every 5 seconds  

---

# 🌐 CLOUD DASHBOARD

<p align="center">
  <img src="docs/images/cloud_dashboard.jpg" width="500" alt="Cloud Dashboard">
</p>

- **Monitor** sensor data remotely  
- **Control** relay appliances via web interface  
- Supports **real-time synchronization with Google Home commands**

---

# 📂 SOFTWARE STRUCTURE


Firmware modules:

- Task scheduling and cloud updates  
- Sensor data acquisition  
- Relay and manual switch control  
- OLED display management  
- Cloud & voice integration logic  

---

## 🧪 TESTING & VALIDATION

- Verified relay response to **voice commands via Google Home**  
- Manual switch tested for immediate override  
- Sensor readings validated against standard DHT11 and LDR values  
- OLED display cycles and cloud dashboard updates verified  
- System stable under continuous operation  

---

## 🔮 FUTURE IMPROVEMENTS

- Integrate **multiple relays** for multi-appliance control  
- Add **mobile app interface** for remote control  
- Implement **automation rules** (time-based, light-based)  
- Enhance **security with token-based cloud access**  

---

## 👥 TEAM / AUTHOR

- Sreeram Raman – S3 ECE Student, IoT & Home Automation Enthusiast  




