# 🌍 IoT Weather Monitoring System using ESP8266 ☁️🌡️

## 📌 Introduction
This project is an **IoT-based Weather Monitoring System** that collects and uploads real-time weather data to **ThingSpeak** using an **ESP8266 Wi-Fi module**. The system measures **temperature, humidity, air quality, atmospheric pressure, and light intensity** and transmits the data over the internet.

## ✨ Features
✅ Measures **Temperature** and **Humidity** using **DHT11 sensor**  
✅ Monitors **Air Quality** using **MQ-135 sensor**  
✅ Detects **Light Intensity** using **LDR sensor**  
✅ Records **Atmospheric Pressure** using **BMP180 sensor**  
✅ Displays real-time data on an **LCD Display**  
✅ Sends data to **ThingSpeak Cloud** for remote monitoring  

## 🔧 Hardware Requirements
- 🛠️ **ESP8266 Wi-Fi Module**
- 🛠️ **Arduino UNO**
- 🌡️ **DHT11 Temperature & Humidity Sensor**
- 🏭 **MQ-135 Air Quality Sensor**
- 🌤️ **BMP180 Barometric Pressure Sensor**
- ☀️ **LDR (Light Dependent Resistor)**
- 📟 **16x2 LCD Display with I2C Interface**
- 🔋 **Power Supply (5V)**

## 💻 Software Requirements
- **Arduino IDE** (for programming the ESP8266)
- **ThingSpeak API** (for IoT data visualization)
- **Required Libraries:**
  - `ESP8266WiFi.h`
  - `ThingSpeak.h`
  - `Wire.h`
  - `dht.h`
  - `BMP180.h`
  - `LiquidCrystal_I2C.h`

## 🚀 Installation and Setup
### 1️⃣ Install Required Libraries in Arduino IDE
Go to **Sketch > Include Library > Manage Libraries**, and install:
- 📌 `ESP8266WiFi`
- 📌 `ThingSpeak`
- 📌 `DHT Sensor Library`
- 📌 `Adafruit BMP180`
- 📌 `LiquidCrystal I2C`

### 2️⃣ Configure Wi-Fi and ThingSpeak API
Update the following in `ESP8266.ino`:
```cpp
char ssid[] = "YOUR_WIFI_SSID"; 
char pass[] = "YOUR_WIFI_PASSWORD"; 
unsigned long Channel_ID = YOUR_CHANNEL_ID;
const char *myWriteAPIKey = "YOUR_API_KEY";
```

### 3️⃣ Upload the Code to ESP8266
1. 🔌 Connect ESP8266 to PC using USB-to-serial adapter.
2. ⚙️ Select **ESP8266 Board** in **Tools > Board**.
3. 🔍 Choose the correct **COM Port**.
4. 🚀 Click **Upload**.

### 4️⃣ Monitor Data on ThingSpeak
1. 🌎 Open **ThingSpeak** and navigate to your channel.
2. 📊 View real-time sensor data updates.


---
🌎 This project was developed as part of an **IoT Weather Monitoring System** to provide real-time environmental data for smart applications. 🚀

