# ESP32 Smart Water Meter (IWS / Municipal Supply)

This is the official ESPHome configuration and Home Assistant logic for the DIY Smart Water Meter project.

It is designed specifically for **Intermittent Water Supply (IWS)** scenarios common in regions like India, where pumps must detect water availability in unpressurized lines to avoid dry runs.

## 📖 Full Guide & Tutorial
**[Click here for the Step-by-Step Guide on BabaBuilds.com](https://bababuilds.com/blog/esp32-smart-water-meter-diy/)** *(Check the article for wiring instructions, 3D printed case files, and the physics behind the "Priming Window" logic.)*

## 🛠 Hardware Required
* **Microcontroller:** ESP32 Dev Kit V1 (NodeMCU)
* **Sensor:** YF-G1 DN25 Water Flow Sensor (or DN20 for smaller pipes)
* **Power:** 5V DC Supply
* **Relay:** 5V Single Channel Relay (High/Low trigger)

## ⚡ Features
* **Dry Run Protection:** Automatically cuts off the pump if flow is < 5LPM after priming.
* **Total Volume Tracking:** Tracks daily water usage in Liters.
* **Home Assistant Integration:** Native API support.

## 🔧 Installation
1.  Copy `secrets.yaml.example` to `secrets.yaml` and fill in your WiFi details.
2.  Flash `water-meter.yaml` to your ESP32.
3.  Copy the automation logic from the `/home-assistant` folder to your HA config.

## 📄 License
MIT License - feel free to modify and share!
