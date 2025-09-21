# Object Counter using ESP32-CAM and FTDI Module

## 📌 Introduction
In industries, retail stores, and automation applications, counting objects is crucial for tracking inventory, optimizing processes, and ensuring accuracy.  
This project implements an **Object Counter** using **ESP32-CAM**, a low-cost Wi-Fi-enabled microcontroller with a camera module, to detect and count objects using image processing.

---

## 🎯 Objectives
- Develop an automated object counter using ESP32-CAM.  
- Use image processing techniques to detect and count objects.  
- Display the counted objects on a web interface using ESP32’s built-in server.  
- Interface the ESP32-CAM with an FTDI Module for programming and debugging.  

---

## 🛠️ Components Required
| Component      | Description |
|----------------|-------------|
| **ESP32-CAM** | Wi-Fi-enabled microcontroller with OV2640 camera |
| **FTDI Module** | USB to TTL serial converter for programming ESP32-CAM |
| **Power Supply** | 5V DC source |
| **IR LEDs (optional)** | Enhances object detection in low light |
| **Resistors & Capacitors** | Basic circuit stability elements |
| **Jumper Wires** | For connections |

---

## ⚡ Working Principle
1. The ESP32-CAM captures images of objects passing in front of its camera.  
2. The image processing algorithm detects objects (via edge detection or color thresholding).  
3. A counting algorithm updates the object count based on movement or detected boundaries.  
4. The ESP32-CAM hosts a **web server**, displaying the live object count.  
5. The FTDI module is used to program and debug the ESP32-CAM.  

---

## 🔌 Circuit Connections
### ESP32-CAM ↔ FTDI Module
| ESP32-CAM Pin | FTDI Module Pin |
|---------------|-----------------|
| U0TXD | RX |
| U0RXD | TX |
| GND   | GND |
| 5V    | VCC (5V) |
| GPIO0 | GND (only for programming mode) |

### ESP32-CAM ↔ Power Supply
- **5V pin** → 5V Power Source  
- **GND pin** → Power Source GND  

---

## 💻 Software Implementation
### Tools Required
- Arduino IDE (for programming ESP32-CAM)  
- ESP32 board package (installed in Arduino IDE)  
- OpenCV (optional, for advanced image processing)  
- Web Server Code (to host object count on webpage)  

👉 [Code Link]() (add your code link here)

---

## 🌐 Web Server Interface
- The ESP32-CAM runs a lightweight web server.  
- Real-time object count is displayed on the webpage.  
- AJAX requests fetch the latest count seamlessly.  

---

## ✅ Advantages
- Low-cost implementation  
- Wireless monitoring via Wi-Fi  
- No additional hardware sensors required  

---

## 🚀 Applications
- Factory automation → counting products on assembly line  
- Retail stores → tracking items on shelves  
- Smart parking → counting available parking slots  

---

## 🔮 Future Improvements
- Machine Learning integration for higher accuracy  
- Cloud storage for analytics and history tracking  
- Battery-powered portable version  

---

## 🏁 Conclusion
The **ESP32-CAM Object Counter** is a simple yet effective automation project that enables real-time object counting using a camera module.  
Its integration with a web server allows monitoring from any device connected to the same network.  

---

📢 *Developed at UVCE MARVEL Lab*
