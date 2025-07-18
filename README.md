# IOT_4thsem_pbl

# Smart Helmet for Rider Safety 

An IoT-based Smart Helmet designed to enhance rider safety through accident detection, helmet usage monitoring, and emergency notifications.


# Project Overview

This project leverages sensors and IoT technology to ensure both accident detection and helmet compliance for motorbike riders. It monitors for collisions and detects if the rider is wearing a helmet, sending real-time alerts to concerned authorities or emergency contacts via the internet.



# Features

- Helmet Detection: Uses an RFID module embedded inside the helmet to ensure the rider is wearing it before starting the vehicle.
- Accident Detection: An MPU6050 (accelerometer + gyroscope) senses sudden impacts and tilt, indicating accidents.
- Emergency Alerts: NodeMCU sends automatic notifications to pre-configured emergency contacts if an accident is detected.
- Buzzer Alerts: A buzzer provides an immediate audible alert in case of accidents or system issues.
- WiFi Connectivity: Powered by NodeMCU to enable real-time notifications via the internet.



# Hardware Requirements

| Component      | Quantity |
| -------------- | -------- |
| NodeMCU ESP8266 | 1 |
| MPU6050 Accelerometer + Gyroscope | 1 |
| RFID Reader (RC522) | 1 |
| RFID Tag | 1 |
| Buzzer | 1 |
| Breadboard and Jumper Wires | As required |
| Power Source (USB or Battery) | 1 |



# Software & Libraries

- Arduino IDE
- Libraries:
  - Wire.h
  - Adafruit_MPU6050
  - SPI.h
  - MFRC522.h
  - ESP8266WiFi.h
  - ThingSpeak 
- WiFi Credentials for connectivity
- Emergency contact configuration


# Working Mechanism

1. Helmet Check: When the vehicle is turned on, the RFID reader checks for the presence of an RFID tag inside the helmet.
2. Motion Monitoring: MPU6050 continuously monitors the rider's motion.
3. Accident Detection: Sudden high G-force or tilt triggers accident detection.
4. Alert System: NodeMCU sends an emergency alert with location (if integrated with GPS) or predefined message via the internet.
5. Buzzer: Sounds for immediate local alerts.



# Future Improvements

- Integrate GPS for location tracking
- Mobile app notifications
- Fall detection improvements using advanced ML algorithms
- Battery optimization for longer operation


# Author

- Jashaswi Mahapatra



