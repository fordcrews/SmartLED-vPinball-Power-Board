# SmartLED & Pinball Power Board v1

## Overview
SmartLED v1 is a modular, ATX-powered breakout board designed for ESP32-based lighting, solenoid, and accessory control projects such as:

- Virtual Pinball Machines  
- Holiday Light Shows  
- Aquarium Automation  
- Home Decor Lighting Systems

## Features

### 🔌 ATX/Mini-ITX Power Supply Input
- Standard 24-pin ATX connector
- `PS_ON#` control via MOSFET (GPIO or jumper selectable)
- Uses `+5VSB` to power ESP32 independently of main rails

### 🧠 ESP32 DevKitC Integration
- Supports 30-pin DevKitC boards
- Powered by +5VSB with onboard regulation
- Breakout header for unused GPIOs

### 💡 Buffered LED Outputs (8x)
- 3-pin JST outputs with:
  - AHCT125 level shifters (3.3V to 5V)
  - Selectable 5V or 12V via jumper
  - Fused output per channel

### 🧰 Dual Terminal Access
- Breadboard header (J10) and cabinet terminal block (J11)
- Shared pinout, use either or both

### 🧩 GPIO Expansion
- I²C header (GND, VCC, SDA, SCL)
- Additional GPIOs for sensors, encoders, buttons, etc.

### 🔋 MOSFET Driver Sockets
- 2–4 TO-220 MOSFET slots (e.g. IRLZ44N)
- Gate control via GPIO or jumper
- Voltage selectable (5V/12V AUX)
- For solenoids, fans, relays, motors, etc.

### 🔌 Power Outputs
- USB-C / Micro USB 5V **outputs**
- 5V/12V Barrel jack **outputs**
- Drive external Pi, LED drivers, amps, etc.

### ⚡ Cabinet Power Switch Output
- Optional switched line to control cabinet-wide power
- Triggered via ESP32 or logic jumper

## Optional / Phase 2 Ideas
- Break-off compact section
- Raspberry Pi header (Zero/Full support)
- OLED display pinout for power/usage stats
- Software-based PSU shutdown/watchdog

## Design Goals
- One ATX cable powers your entire rig
- Clean, modular, safe wiring
- Minimalist or advanced builds supported
- Great for compact lighting builds or full-featured pinball control systems

---

📁 PCB, schematic, BOM, and KiCad project files coming soon!
