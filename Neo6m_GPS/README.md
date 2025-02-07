# esp-idf-neo6m-gps

## Overview  
This project provides an ESP-IDF 5.4-based implementation for interfacing with the **Neo-6M GPS** module using UART communication. The software reads **NMEA** sentences, extracts **GPGLL** data, and converts it into usable latitude and longitude coordinates.

## Features  
- UART-based GPS data reception.  
- Parsing of `$GPGLL` NMEA sentences to extract **latitude** and **longitude**.  
- Automatic conversion from **NMEA format (DDMM.MMMM) to decimal degrees (DD.DDDDDD)**.  
- Provides functions to fetch the latest valid GPS coordinates.  
- Logs GPS data using **ESP-IDF logging** (`ESP_LOGI`).  

## Hardware Requirements  
- **ESP32 Development Board**  
- **Neo-6M GPS Module**  
- **UART connection:**  
  - **TX (GPS)** → **GPIO17 (ESP32)**  
  - **RX (GPS)** → **GPIO16 (ESP32)**  
  - **GND (GPS)** → **GND (ESP32)**  
  - **VCC (GPS)** → **3.3V/5V (ESP32)**  

## Software Requirements  
- **ESP-IDF 5.4 or later**  
- **CMake & Ninja build system**  
- **Serial monitor tool (e.g., `idf.py monitor`)**  

