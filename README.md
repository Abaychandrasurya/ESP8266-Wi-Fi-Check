# ESP8266 Wi-Fi Connection Display with OLED

This simple project uses an **ESP8266** microcontroller and an **SSD1306 OLED display** to show the Wi-Fi connection status and the device’s local IP address. It provides a visual confirmation on the OLED screen once the device successfully connects to a Wi-Fi network.

## 📷 Preview

> ![Example OLED Display](https://via.placeholder.com/128x64?text=WiFi+Connected)  
> ![image](./image1.png)

## 📦 Features

- Connects to a Wi-Fi network using hardcoded SSID and password
- Displays:
  - "Connecting to WiFi..." during connection attempt
  - "WiFi connected!" and local IP address upon successful connection

## 🔧 Hardware Required

- ESP8266 development board (e.g., NodeMCU, Wemos D1 Mini)
- SSD1306 128x64 I2C OLED display
- Jumper wires
- Breadboard (optional)

## 🧠 Libraries Used

- [`ESP8266WiFi`](https://arduino-esp8266.readthedocs.io/en/latest/)
- [`Adafruit_GFX`](https://github.com/adafruit/Adafruit-GFX-Library)
- [`Adafruit_SSD1306`](https://github.com/adafruit/Adafruit_SSD1306)

Install these libraries through the Arduino Library Manager.

## 🔌 Wiring

| OLED Pin | ESP8266 Pin |
|----------|-------------|
| VCC      | 3.3V        |
| GND      | GND         |
| SDA      | D2 (GPIO4)  |
| SCL      | D1 (GPIO5)  |

## 📜 Code

> See `main.ino` for the full source code.

## 📈 Future Improvements (Optional Ideas)

- Display signal strength (RSSI)
- Add auto reconnect logic
- Support for multiple Wi-Fi networks
- Show connection status in the `loop()`

---

## 📬 About

This project provides a minimal yet practical example of using an ESP8266 to connect to Wi-Fi and display network status on a 0.96" SSD1306 OLED. It's a great starting point for more advanced IoT projects where network visibility is important.
