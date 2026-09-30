# 🏫 Intelligent Classroom Monitoring and Management System

### 💡 An IoT-Based Smart Classroom Automation Project

An intelligent classroom monitoring system that combines **IoT, sensor technology, Python, and machine learning** to monitor classroom environmental conditions and support automated control of lights and fans.

🎥 **Project Demo:** [Watch the Demo Video](PASTE_YOUR_GOOGLE_DRIVE_LINK_HERE)

---

## 🌟 About the Project

Traditional classrooms often rely on manual operation of lights and fans, which can lead to unnecessary energy consumption and limited awareness of classroom conditions.

The **Intelligent Classroom Monitoring and Management System** aims to address these challenges through IoT-based monitoring and automation.

Using a NodeMCU ESP8266, environmental sensors, a Python backend, and a dashboard, the system collects sensor readings, monitors classroom conditions, and supports automated appliance control based on the implemented logic.

Our goal is to contribute to a smarter, more efficient, and technology-driven classroom environment. 🚀

---

## ✨ Key Features

* 🌡️ **Temperature & Humidity Monitoring** — Monitors classroom environmental conditions.
* 💡 **Light Intensity Detection** — Measures ambient light levels to support lighting automation.
* 🚶 **Motion Detection** — Detects movement or presence using connected sensors.
* 🌫️ **Gas Detection** — Monitors gas-sensor readings and supports alerts.
* ⚡ **Smart Appliance Control** — Supports automated operation of lights and fans.
* 📊 **Interactive Dashboard** — Provides a convenient interface for monitoring available readings and system status.
* 🗄️ **Data Storage** — Uses SQLite for local data persistence.
* 🤖 **Machine Learning Integration** — Includes model files and training scripts for fan and light control.
* 📡 **IoT Connectivity** — Connects the hardware prototype with the software components.

---

## 🏗️ System Architecture

The project consists of the following layers:

1. **Sensing Layer:** Collects temperature, humidity, light, gas, and motion-related readings.
2. **Controller Layer:** The NodeMCU ESP8266 interfaces with the connected sensors and hardware.
3. **Backend Layer:** The Flask application handles the supported application logic and data processing.
4. **Database Layer:** SQLite provides local data storage.
5. **Dashboard Layer:** Streamlit provides a dashboard for monitoring the system.
6. **Actuation Layer:** Connected output devices, such as lights and fans, can be controlled according to the configured logic.

🔄 These components work together to support classroom monitoring and automation.

---

## 🔧 Hardware Requirements

| Component                    | Purpose                              |
| ---------------------------- | ------------------------------------ |
| 🔌 NodeMCU ESP8266           | Main IoT microcontroller             |
| 🌡️ DHT11 Sensor             | Temperature and humidity monitoring  |
| 🌫️ MQ135 Sensor             | Gas/air-quality indication           |
| 💡 LDR Sensor                | Light intensity detection            |
| 🚶 PIR/IR Sensors            | Motion or presence detection         |
| ⚡ Relay Module               | Switching connected electrical loads |
| 💡 Light and Fan             | Controlled output devices            |
| 🔋 Power Supply              | Powers the prototype                 |
| 🧩 Breadboard & Jumper Wires | Circuit assembly and connections     |

*Note: Confirm the actual sensors and components used in your final hardware setup before reproducing the project.*

---

## 💻 Technologies Used

| Technology                | Application                        |
| ------------------------- | ---------------------------------- |
| 🟢 NodeMCU ESP8266        | IoT hardware and connectivity      |
| ⚙️ Embedded C/C++         | Microcontroller firmware           |
| 🐍 Python                 | Backend and model development      |
| 🌐 Flask                  | Backend application                |
| 📊 Streamlit              | Monitoring dashboard               |
| 🗄️ SQLite                | Database                           |
| 🧠 Machine Learning       | Fan/light model files and training |
| 🎨 HTML, CSS & JavaScript | Frontend interface                 |
| 🛠️ Arduino IDE           | Firmware development               |
| 🐙 Git & GitHub           | Version control and collaboration  |

---

## 📁 Project Structure

```text
Intelligent-Classroom-Monitoring-Hackathon/
│
└── miniprj/
    ├── backend/
    │   ├── app.py
    │   ├── models.py
    │   ├── utils.py
    │   ├── requirements.txt
    │   ├── database.db
    │   ├── fan.pkl
    │   └── light.pkl
    │
    ├── dashboard/
    │   └── dashboard.py
    │
    ├── frontend/
    │   ├── index.html
    │   ├── scripts.js
    │   └── styles.css
    │
    ├── libraries/
    │
    ├── ml_model/
    │   ├── train_fan_model.py
    │   └── train_light_model.py
    │
    ├── miniprj1/
    │   └── miniprj1.ino
    │
    └── sketch_aug18a/
        └── sketch_aug18a.ino
```

---

## 🚀 Getting Started

Follow these steps to run the software locally.

### 📌 Prerequisites

Make sure you have installed:

* Python and pip
* Git
* Arduino IDE
* NodeMCU ESP8266 board support
* Required hardware libraries and sensors

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/mahendramanikanta/Intelligent-Classroom-Monitoring-Hackathon.git
```

Navigate to the project directory:

```bash
cd Intelligent-Classroom-Monitoring-Hackathon
```

### 2️⃣ Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

On macOS/Linux:

```bash
source .venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r miniprj/backend/requirements.txt
```

### 4️⃣ Run the Flask Backend

```bash
python miniprj/backend/app.py
```

Check the terminal for the address and port used by the application.

### 5️⃣ Launch the Dashboard

Open a new terminal in the repository root and activate the virtual environment if necessary.

Run:

```bash
streamlit run miniprj/dashboard/dashboard.py
```

Open the local URL displayed in your terminal.

### 6️⃣ Upload the Firmware

1. Open the appropriate `.ino` file in Arduino IDE.
2. Select the NodeMCU ESP8266 board and the correct COM port.
3. Configure Wi-Fi credentials and the backend address if required.
4. Verify sensor pin assignments and relay connections.
5. Upload the firmware and inspect the Serial Monitor.

⚠️ **Important:** The repository contains multiple firmware sketches. Select the one that matches your actual hardware wiring and configuration.

---

## 🧪 Testing and Observations

The prototype is designed to demonstrate:

* 🌡️ Environmental sensor monitoring.
* 🚶 Motion detection.
* 🌫️ Gas-sensor alerts.
* 💡 Automated lighting based on the configured logic.
* 🌀 Fan control based on the implemented conditions.
* 📊 Dashboard-based system monitoring.

The actual results depend on sensor calibration, hardware connections, firmware configuration, and network availability.

---

## ⚠️ Limitations

* Sensor accuracy depends on calibration and the quality of the hardware.
* Automation depends on the configured thresholds and control logic.
* Gas-sensor readings are indicative and are not a substitute for certified safety equipment.
* The current prototype's energy savings have not been quantified with numerical measurements.
* Remote access requires additional network configuration and appropriate security measures.

---

## 🔮 Future Enhancements

* 📈 Add historical data visualization and reporting.
* ⚡ Measure and compare energy consumption before and after automation.
* 📱 Develop a mobile-friendly monitoring interface.
* 🏫 Extend the system to support multiple classrooms.
* 🔔 Add improved alert notifications.
* 🔐 Implement secure remote access and user authentication.
* 🧠 Explore predictive analytics for more adaptive classroom automation.

---

## 🎥 Project Demonstration

Want to see the system in action?

▶️ **[Click Here to Watch the Project Demo](PASTE_YOUR_GOOGLE_DRIVE_LINK_HERE)**

*The demo video showcases the physical prototype and the available system functionality.*

---

## 👨‍💻 Developer

**Manikanta**

🔗 GitHub: [@mahendramanikanta](https://github.com/mahendramanikanta)

---

## 🏁 Conclusion

The **Intelligent Classroom Monitoring and Management System** demonstrates how IoT sensors, embedded systems, backend technologies, and a monitoring dashboard can be integrated to support smarter classroom management.

The project serves as a prototype for exploring environmental monitoring, occupancy-aware automation, and more efficient classroom operations.

🚀 **Building smarter classrooms through technology!**

---

⭐ If you find this project interesting, consider giving the repository a star!
