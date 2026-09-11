# SensorGrid Dashboard + ESP32 LED Blink

A complete IoT project featuring a responsive sensor monitoring web dashboard and an ESP32 microcontroller simulation.

---

## 🌐 Part 1: SensorGrid Dashboard

A responsive IoT sensor monitoring dashboard built using semantic HTML5 and modern CSS (Flexbox and Grid).

### Features
- **Semantic HTML5 Architecture**: Structured with standard tags including `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<table>`, and `<footer>`.
- **Navigation Bar**: Quick-access links styled using CSS Flexbox.
- **Sensor Cards (CSS Grid)**: Displays live IoT metrics (Temperature, Humidity, Air Quality, Light) in an organized 4-column grid layout.
- **Sensor Status Indicators**: Visual status indicators (Active/Inactive) with color-coded badges.
- **Sensor Status Table**: Tabular view of sensor values, units, and operating status.
- **Responsive Design**: Fully responsive layout adapting smoothly from desktop to mobile screens via media queries.

### How to Run Dashboard
1. Open `index.html` directly in any web browser, or serve it using Python:
   ```bash
   python -m http.server 8085
   ```
2. Visit `http://localhost:8085` in your browser.

---

## ⚡ Part 2: ESP32 LED Blink Simulation (Wokwi)

An ESP32 microcontroller simulation in Wokwi where an LED connected to GPIO 2 blinks ON/OFF every 1 second, printing status messages to the Serial Monitor at 115200 baud.

### Circuit Connections
- **LED Anode (`A`)** &rarr; `GPIO 2` (`esp:2`)
- **LED Cathode (`C`)** &rarr; `GND` (`esp:GND.1`)

### How to Run Simulation
1. Open `diagram.json` in VS Code with the Wokwi extension.
2. Press `F1` or `Ctrl + Shift + P` and select **Wokwi: Start Simulator** (or click the green Play button).

---

## 📁 Project Structure

```
├── index.html       # Semantic HTML5 dashboard layout
├── style.css        # Flexbox, Grid, and responsive styling
├── sketch.ino       # ESP32 Arduino sketch for LED blinking
├── diagram.json     # Wokwi circuit diagram & connections
├── wokwi.toml       # Wokwi simulation configuration
├── platformio.ini   # PlatformIO build configuration
├── .gitignore       # Git ignore rules
└── README.md        # Project documentation
```
