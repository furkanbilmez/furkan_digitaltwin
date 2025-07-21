# Digital Twin for Conveyor Belt System in a Marble Factory

This project is a real-time digital twin of a conveyor belt system in a marble factory. It integrates programmable logic control (PLC), sensor input, MQTT communication, and a Unity-based digital visualization. The system simulates and monitors the physical conveyor belt process using digital technologies, reflecting the principles of Industry 4.0.

---

## 🚀 Project Objectives

- Develop a working conveyor belt controlled by PLC.
- Integrate photoelectric sensors to detect object presence.
- Use ESP32-CAM for real-time image capture and monitoring.
- Send and receive data through MQTT.
- Create a Unity-based digital twin that visualizes the system status and object movement.
- Enable real-time synchronization between physical and digital systems.

---

## 🧠 Technologies Used

| Technology | Purpose |
|------------|---------|
| **PLC (SoMachine)** | Controls conveyor, timer, counter, and sensor logic |
| **ESP32-CAM** | Captures image and distance data |
| **MQTT** | Communication between hardware and digital twin |
| **Unity 3D** | Digital twin visualization |
| **Node-RED** | Data flow visualization (optional) |
| **Python** | For sensor communication (if needed) |

---

## 🏗️ System Architecture


---

## ⚙️ System Components

- **XT218A1PCM12 Sensor**: Used to detect metal presence on the conveyor.
- **XUB5BPANL2 Sensor**: General object detection sensor.
- **PLC Program**: Controls conveyor motor, stops with counter, resets with timer.
- **Unity Interface**: Shows the virtual conveyor, object flow, sensor trigger in real time.

---

## ✅ Status

🔧 In progress — ESP32 integration & Unity twin testing ongoing.

---

## 📌 Future Work

- Add dashboard with live MQTT values.
- Implement alert system for jammed conveyor.
- Connect database for storing object movement history.

---

## 📄 License

MIT License.
