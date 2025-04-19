# RuuviTag-Calf-Monitoring

A Node-RED-based monitoring system for tracking calf movement and behavior using **RuuviTag** Bluetooth sensors and low-cost Raspberry Pi-based gateways. This project explores open-source, scalable, and affordable methods for **precision livestock monitoring**, starting with **dairy/beef calves** aged 2–10 weeks.

---

### 📦 Project Goals

- 🐄 Monitor calf movement and orientation using BLE tags
- 📐 Track posture (lying, standing, active bursts)
- 📡 Decode and forward RuuviTag data via MQTT
- 🌐 Centralize data on a remote server for analysis and dashboards
- 🧠 Enable future behavior classification using AI or rule-based logic

---

### 🧰 Hardware Setup

| Component | Role |
|----------|------|
| 📶 Raspberry Pi Zero 2 W | BLE gateways scanning for RuuviTags, forwarding data via MQTT using **Ruuvi Go Gateway** software |
| 🏷️ RuuviTag Sensors | Mounted on calf collars to track movement & orientation |
| 🖥️ Remote Server | Host Node-Red, MQTT Broker, InfluxDB and Grafana |

---

### 🛠️ Software Stack

- **Node-RED** – data parsing, logic, visualization
- **MQTT Broker** – receives BLE data from gateways
- **Ruuvi Go Gateway** – runs on Raspberry Pi Zero 2 W to forward RuuviTag data
- **InfluxDB + Grafana**  – logging and historical visualization

---

### 📊 Project Functions

- Parse BLE Format 5 broadcasts from RuuviTags
- Extract acceleration, orientation and battery data
- Push real-time readings to the MQTT broker
- Visualize calf activity across pens
- Lay foundation for AI-driven behavioral insights

---

### 🚧 Current WIP Status

This project is a reboot of an earlier prototype. Flows will be rebuilt with:
- Streamlined MQTT BLE gateways (Pi Zero 2 W running **Ruuvi Go Gateway** software)
- Improved parsing logic
- Clean, modular dashboards and flow structure
- Focus on practical farm conditions (pens, gateway range, calf posture, enviroment monitoring)

---

### 📈 Future Plans

- Support behavior tagging for ML training
- gateway triangulation to determin position in pens
- Integrate with optional video-based AI systems for validation
- Expand to weaned calf groups or heifer monitoring

---

### 👨‍🔧 Maintainer

Farmer-Ed – [@Farmer-Eds-Shed](https://github.com/Farmer-Eds-Shed)  
📍 County Meath, Ireland
