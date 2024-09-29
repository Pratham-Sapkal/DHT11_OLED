# Temperature and Humidity Measurement using DHT11, OLED Display, and Arduino Nano

## Overview
This project involves measuring temperature and humidity using the DHT11 sensor, displaying the data on an OLED display, and using an Arduino Nano as the controller.

## Components Required
- Arduino Nano
- DHT11 Temperature and Humidity Sensor
- 0.96" OLED Display (I2C interface)
- Jumper Wires
- Breadboard
- USB Cable

## Circuit Diagram
Connect the components as follows:

1. **DHT11 Sensor:**
   - VCC to 5V of Arduino Nano
   - GND to GND of Arduino Nano
   - Data Pin to Digital Pin D2 of Arduino Nano

2. **OLED Display:**
   - VCC to 3.3V of Arduino Nano
   - GND to GND of Arduino Nano
   - SCL to A5 of Arduino Nano
   - SDA to A4 of Arduino Nano

## Libraries Required
Install the following libraries in the Arduino IDE:
1. `DHT Sensor Library` by Adafruit
2. `Adafruit Unified Sensor` library
3. `Adafruit GFX Library`
4. `Adafruit SSD1306` library

To install libraries:
1. Open Arduino IDE.
2. Go to **Sketch** > **Include Library** > **Manage Libraries**.
3. Search for the above libraries and click **Install**.

###  Upload the Given Code

## Notes
- Ensure the connections are secure to avoid incorrect readings.
- The OLED display I2C address is set to 0x3C. Modify the code if your OLED display has a different address.

## Troubleshooting
- If the display does not turn on, verify the I2C connections (SCL and SDA) and the I2C address in the code.
- If the DHT11 sensor fails to read data, double-check the wiring and ensure the data pin is connected properly.
