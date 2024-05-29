# Air Quality Monitoring System

## Description
This project is an air quality monitoring system that uses sensors to measure the levels of CO (carbon monoxide), temperature, humidity, and PM2.5 dust particles. The data is displayed on an OLED screen and can be monitored remotely via the Blynk application.

## Components Used
- ESP32
- CO Sensor (MQ-7)
- DHT11 Sensor (temperature and humidity)
- PM2.5 Dust Sensor
- SSD1306 OLED Display
- Buzzer
- LEDs (red, yellow, green)
- Blynk Application

## Installation

### 1. Hardware
Connect the sensors and OLED display to the ESP32 as follows:
- MQ-7: A0 pin connected to pin 33 of the ESP32
- DHT11: Signal pin connected to pin 4 of the ESP32
- PM2.5 Dust Sensor: Signal pin connected to pin 35 of the ESP32, LED power pin of the sensor connected to pin 16 of the ESP32
- OLED Display: Connected via I2C (SDA to pin 21, SCL to pin 22)
- Buzzer: Connected to pin 26 of the ESP32
- LEDs: Red LED connected to pin 12, yellow LED connected to pin 14, green LED connected to pin 27 of the ESP32

### 2. Software
1. Install [Arduino IDE](https://www.arduino.cc/en/Main/Software).
2. Add the ESP32 board to the Arduino IDE by following [this guide](https://github.com/espressif/arduino-esp32/blob/master/docs/arduino-ide/boards_manager.md).
3. Install the necessary libraries:
   - Adafruit GFX Library
   - Adafruit SSD1306
   - Adafruit Unified Sensor
   - DHT sensor library
   - Blynk
   - WiFi
You can install these libraries through the Library Manager in the Arduino IDE (Sketch > Include Library > Manage Libraries).

4. Clone this repository to your computer:
   ```sh
   git clone https://github.com/yourusername/AirQualityMonitoringSystem.git
