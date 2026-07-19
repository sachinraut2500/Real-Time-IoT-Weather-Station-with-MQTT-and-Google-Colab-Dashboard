# 🌤️ Real-Time IoT Weather Station with MQTT & Python Dashboard

This project uses an **ESP32 or ESP8266** to send real-time **temperature and humidity** data from a DHT sensor to a public **MQTT broker**, and visualizes that data in real-time using a **Python-based dashboard** with `matplotlib`.

------

## 🚀 Features

- 📡 IoT device sends temperature/humidity via MQTT.
- 📊 Real-time data visualization using Python.
- ✅ Works in both Google Colab and local Python environments.
- Modular, extensible, and beginner-friendly.

-----

## 🛠 Hardware Require

- ESP32 or ESP8266 microcontroller
- DHT11 or DHT22 sensor
- Jumper wires
- Breadboard
- Wi-Fi connection

----

## 🧰 Software Requirements

### On ESP32/ESP8266:
- [Arduino IDE](https://www.arduino.cc/en/software)
- DHT sensor library
- PubSubClient library

### On PC / Server:
- Python 3.x
- Libraries:
  - `paho-mqtt`
  - `matplotlib`
  - `pandas`

> The script auto-installs missing Python dependencies when run.

---

## 📡 MQTT Configuration

| Parameter  | Value               |
|------------|---------------------|
| Broker     | `broker.hivemq.com` |
| Port       | `1883`              |
| Topic      | `iot/weatherstation` |
| Auth       | None (public)       |

---

## 📂 Files Included

- `esp32_mqtt_code.ino` – Arduino code for ESP32/8266
- `iot_weather_dashboard.py` – Real-time Python dashboard
- `README.md` – Project documentation

---

## 🔧 Setup Instructions

### 1. Flash the ESP32/ESP8266
- Open `esp32_mqtt_code.ino` in Arduino IDE
- Replace `YOUR_WIFI_SSID` and `YOUR_WIFI_PASSWORD`
- Upload to board

### 2. Run Python Dashboard
- Open `iot_weather_dashboard.py`
- Run the script:
```bash
python iot_weather_dashboard.py
