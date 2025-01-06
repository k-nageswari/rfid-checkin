# RFID Based Attendance System with Servo and ThingSpeak

This project demonstrates an RFID-based attendance system using the **ESP8266** microcontroller. The system records attendance and opens a servo-controlled door for authorized individuals. Attendance data is uploaded to **ThingSpeak**, an IoT platform.

## Features
- **RFID Scanning**: Scans RFID tags to authenticate users.
- **Servo Motor**: Controls a door lock mechanism.
- **Buzzer**: Emits a sound when a user scans their RFID card.
- **LCD Display**: Displays user information (Name and Roll Number).
- **ThingSpeak Integration**: Sends attendance data to ThingSpeak for remote monitoring.

## Hardware Requirements
- **ESP8266** (e.g., NodeMCU, Wemos D1 Mini)
- **RFID Reader** (MFRC522 or compatible)
- **Servo Motor** (for door control)
- **Buzzer**
- **LCD 16x2 with I2C**
- **Wires and Breadboard**

## Software Requirements
- **Arduino IDE**: Ensure that you have the ESP8266 board manager installed.
- **Libraries**:
  - `ESP8266WiFi`
  - `ThingSpeak`
  - `SoftwareSerial`
  - `LiquidCrystal_I2C`
  - `Servo`

## Pin Mapping
- **D7**: RFID Reader (RX)
- **D8**: RFID Reader (TX)
- **D5**: Buzzer
- **D6**: Servo Motor
- **D1**: SCL (I2C for LCD)
- **D2**: SDA (I2C for LCD)


## Code Explanation

### Key Sections:

- **WiFi Setup**: Connects to your Wi-Fi network.
- **RFID Scanning**: Reads the RFID tag when scanned and checks against predefined tag IDs.
- **Servo Control**: Opens and closes the door (servo motor).
- **ThingSpeak**: Sends attendance data (Name and Roll Number) to your ThingSpeak channel.
- **LCD Display**: Shows the user information and status.



   
