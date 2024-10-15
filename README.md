# chemo_drug_prep_machine
This project is the firmware for a chemotherapy drug preparation machine using an ESP32 microcontroller. The system interacts with Firebase to receive commands, control servos and stepper motors for various drug preparation actions, and supports over-the-air (OTA) firmware updates.

 ![image](https://github.com/user-attachments/assets/e3cc64b5-5f57-4d80-8760-98f897cbf335)
## Features
- **Wi-Fi Connectivity**: Automatically connects to a Wi-Fi network via Wi-Fi Manager.
- **Firebase Integration**: Listens for user commands from Firebase and triggers corresponding actions (e.g., dosing, purging, collecting).
- **Motor Control**: Controls servo motors for actuating mechanical parts and stepper motors for precise volume dispensing.
- **OTA Updates**: Supports firmware updates via ElegantOTA through a web interface.
- **Real-Time Feedback**: Updates Firebase with the status and feedback of each action (e.g., operation success or failure).
- **Epoch Time**: Uses an NTP server to fetch epoch time for precise time-stamping of operations.
## Hardware Requirements
- ESP32 Board
- Servos: 2x Servo motors 
- Stepper Motor: Controlled via direction and step pins
- Potentiometer: Used for feedback
## Libraries Used
- ESP32Servo
- WiFiManager
- Firebase ESP Client
- ESPAsyncWebServer
- ElegantOTA

