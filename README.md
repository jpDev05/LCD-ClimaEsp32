# 🌦️ LCD Climate ESP32

Project developed using an ESP32 and a 20x4 I2C LCD display to show real-time weather and time information using online APIs.

---

# 📌 Features

✅ Real-time weather monitoring
✅ Current temperature
✅ Feels-like temperature
✅ Air humidity
✅ Cloud coverage
✅ Wind speed
✅ Translated wind direction
✅ Atmospheric pressure
✅ UV index
✅ Real-time clock
✅ Screen navigation using a button
✅ Automatic data updates

---

# 🛠️ Technologies Used

* ESP32
* C++
* Arduino Framework
* PlatformIO
* REST APIs
* I2C 20x4 LCD
* Wi-Fi
* JSON

---

# 📚 Libraries Used

```cpp
#include <WiFi.h>
#include <WiFiClientSecure.h>
#include <HTTPClient.h>
#include <ArduinoJson.h>
#include <Wire.h>
#include <LiquidCrystal_I2C.h>
```

# 📁 Project Structure

```bash
LCD-ClimaEsp32/
│
├── src/
│   └── main.cpp
│
├── include/
├── lib/
├── platformio.ini
└── README.md
```

# 🔌 Hardware Used

## ESP32

Responsible for Wi-Fi connectivity and data processing.

## LCD I2C 20x4

Responsible for displaying weather information.

I2C Address:

```cpp
0x27
```

## Button

Used GPIO:

```cpp
GPIO 0
```

Function:

* Switch display screens

---

# 🌐 APIs Used

## Weather API

https://www.weatherapi.com/

## Time API

https://timeapi.io/

---

# 📥 How to Download the Project

## Option 1 — Using GitHub

Open the terminal and run:

```bash
git clone https://github.com/JP-DEV-2302/LCD-ClimaEsp32-.git
```

Then:

```bash
cd LCD-ClimaEsp32-
```

---

## Option 2 — Download ZIP

1. Open the GitHub repository
2. Click on **Code**
3. Click on **Download ZIP**
4. Extract the folder

---

# 💻 How to Open in VSCode

## 1. Install VSCode

https://code.visualstudio.com/

---

## 2. Install PlatformIO

https://platformio.org/

Or:

* Open VSCode
* Go to Extensions
* Search for:

```txt
PlatformIO IDE
```

* Install it

---

## 3. Open the Project

In VSCode:

```txt
File → Open Folder
```

Select:

```txt
LCD-ClimaEsp32-
```

---

# ⚙️ Configuration

Open:

```cpp
src/main.cpp
```

Change:

```cpp
const char *WIFI_SSID = "YOUR_WIFI";
const char *WIFI_PASSWORD = "YOUR_PASSWORD";
```

---

# 🔑 API Configuration

Replace your API key here:

```cpp
const char *URL_API = "https://api.weatherapi.com/v1/current.json?key=YOUR_API_KEY";
```

---

# 🚀 How to Compile

Inside PlatformIO:

### Build

Compiles the project.

### Upload

Uploads the firmware to the ESP32.

### Monitor

Opens the serial monitor.

---

# 🔄 System Workflow

The ESP32:

1. Connects to Wi-Fi
2. Accesses APIs
3. Receives JSON data
4. Processes information
5. Displays everything on the LCD

---

# 🖥️ Screen System

## Screen 1

* City
* State
* Time
* Weather condition

## Screen 2

* Temperature
* Feels-like temperature
* Humidity
* Cloud coverage

## Screen 3

* Wind
* Direction
* Pressure
* UV index

---

# 🔁 Automatic Updates

Data is automatically updated every:

```txt
30 seconds
```

---

# 🌬️ Wind Direction Translation

The system automatically translates:

```txt
N   -> North
NE  -> Northeast
SW  -> Southwest
W   -> West
```

---

# 🚧 Future Improvements

* Weather forecast
* Charts and graphs
* Web dashboard
* Mobile app
* IoT integration
* Smart LEDs
* Notifications
* AI integration

---

# 👨‍💻 Author

Project developed by João Pedro.

---

# 📜 License

Educational and experimental project.
