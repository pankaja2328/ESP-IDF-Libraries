# MAX4466 Audio Capture with ESP32

This project demonstrates how to capture audio from the **MAX4466 microphone** using the **ESP32** microcontroller. It utilizes the **I2S** interface to read audio data and can optionally transmit the data using **NRF24L01**.

## Features
- Captures audio using **MAX4466** microphone module
- Uses **I2S** for high-quality digital audio processing
- Implements **FreeRTOS tasks** for efficient real-time execution
- Configurable **sampling rate (40 kHz)**
- Optional transmission via **NRF24L01**

## Hardware Requirements
- **ESP32 Development Board**
- **MAX4466 Electret Microphone Module**
- **NRF24L01 Module** (optional for wireless transmission)
- **Connecting Wires**
- **Power Supply (5V or 3.3V)**

## Software Requirements
- **ESP-IDF (Espressif IoT Development Framework)**
- **FreeRTOS (built into ESP-IDF)**
- **I2S and ADC drivers**
- **CMake / Make (for building the project)**

## File Structure
