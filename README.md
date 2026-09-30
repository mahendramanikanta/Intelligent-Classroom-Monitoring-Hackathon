# 🏫 Intelligent Classroom Monitoring and Management System

### 💡 An IoT-Based Smart Classroom Automation and Energy Optimization Project

An intelligent IoT-based classroom monitoring and management system that integrates **NodeMCU ESP8266, environmental sensors, Python, Flask, SQLite, Streamlit, and machine learning** to monitor classroom conditions, automate electrical appliances, and support energy-efficient classroom operations.

⚡ **Key Highlight:** The project targets **up to 35% simulated energy savings** through predictive control of classroom fans, lights, and ventilation based on environmental conditions and occupancy-related sensor inputs.

🎥 **Project Demo:** [Watch the Demo Video](PASTE_YOUR_GOOGLE_DRIVE_LINK_HERE)

---

## 🌟 About the Project

Traditional classrooms often depend on manual operation of lights, fans, and ventilation systems. This can lead to unnecessary electricity consumption when rooms are unoccupied or when appliances continue operating despite changing environmental conditions.

The **Intelligent Classroom Monitoring and Management System** aims to address these challenges by combining Internet of Things (IoT) technology, sensor-based monitoring, machine learning, and automated appliance control.

The system uses a NodeMCU ESP8266 to interface with connected sensors and collect classroom environmental data. A Python-based Flask backend supports application logic and data processing, SQLite provides local data storage, and a Streamlit dashboard provides an interface for monitoring available readings and system status.

Using the configured control logic and available machine-learning components, the system supports intelligent operation of lights and fans. The broader energy-optimization approach also considers ventilation control according to the available sensor inputs and the implemented hardware configuration.

The objective is to reduce unnecessary appliance operation, improve classroom environmental awareness, and explore more efficient use of electricity in educational institutions.

### 🎯 Project Objectives

* 🌡️ Monitor classroom environmental conditions in real time.
* 🚶 Detect movement or occupancy-related activity using connected sensors.
* 💡 Automate classroom lighting based on the implemented control logic.
* 🌀 Support intelligent fan control according to environmental conditions.
* 🌬️ Explore demand-based ventilation control for improved classroom management.
* 📊 Provide a centralized dashboard for monitoring available sensor readings.
* 🗄️ Store application data locally using SQLite.
* ⚡ Evaluate the potential for energy savings through simulated or measured comparisons.

---

## ✨ Key Features

### 🌡️ 1. Environmental Monitoring

The system uses connected environmental sensors to monitor temperature and humidity. These readings help describe classroom conditions and can be used by the configured automation logic.

### 💡 2. Intelligent Lighting Automation

An LDR sensor measures ambient light intensity. The system can use the available light readings and configured thresholds to support automatic lighting decisions, helping avoid unnecessary lighting when it is not required.

### 🚶 3. Occupancy and Motion Detection

PIR/IR sensors provide motion or presence-related inputs. These inputs can help identify periods of classroom activity and support occupancy-aware appliance control.

### 🌀 4. Predictive Fan Control

The project includes machine-learning model files and training scripts for fan control. These components support experimentation with data-driven fan-control decisions based on the features and logic implemented in the project.

### 🌬️ 5. Ventilation Management

The energy-optimization concept includes ventilation control as part of the broader smart-classroom approach. Actual ventilation automation depends on the connected hardware, available sensors, and implemented control logic.

### 🌫️ 6. Gas Detection and Alerts

The gas sensor provides readings that can be monitored by the application. The system supports alerts when configured conditions are met, helping identify readings that may require attention.

### ⚡ 7. Energy Optimization

By coordinating occupancy-related inputs with lighting and fan control, the system aims to reduce unnecessary appliance runtime.

The project uses an energy-saving evaluation approach to explore potential improvements compared with conventional operation.

**Target energy-saving highlight: Up to 35% simulated energy savings**, subject to the assumptions, baseline, and simulation conditions used in the evaluation.

### 📊 8. Monitoring Dashboard

The Streamlit dashboard provides a convenient interface for viewing available readings and system status.

### 🗄️ 9. Local Data Storage

SQLite is used for local persistence of application data, depending on the implemented backend functionality.

### 📡 10. IoT Hardware Integration

The NodeMCU ESP8266 connects the sensor layer with the software components, enabling the prototype to demonstrate an integrated hardware-and-software workflow.

---

## 🏗️ System Architecture

The system is organized into six logical layers.

### 1. Sensing Layer

Collects data from the available environmental and motion-related sensors, including temperature, humidity, light intensity, and gas-sensor readings.

### 2. Controller Layer

The NodeMCU ESP8266 interfaces with the connected sensors and hardware. Firmware handles the configured sensing and communication tasks.

### 3. Backend Layer

The Flask application provides the backend functionality and processes data according to the implemented application logic.

### 4. Data Storage Layer

SQLite supports local data persistence for the application.

### 5. Dashboard Layer

Streamlit provides a monitoring interface for the available readings and system status.

### 6. Automation and Energy Optimization Layer

The control logic uses available sensor inputs and configured conditions to support lighting and fan operation. Predictive control and ventilation optimization are part of the broader energy-efficiency approach, subject to the functions actually implemented in the prototype.

🔄 Together, these layers demonstrate how IoT sensing, backend processing, monitoring, and appliance control can be integrated into a smart-classroom prototype.

---

## 🔧 Hardware Requirements

| Component              | Purpose                                                 |
| ---------------------- | ------------------------------------------------------- |
| 🔌 NodeMCU ESP8266     | Main microcontroller and Wi-Fi connectivity             |
| 🌡️ DHT11 Sensor       | Temperature and humidity monitoring                     |
| 🌫️ MQ135 Sensor       | Gas/air-quality indication                              |
| 💡 LDR Sensor          | Ambient light detection                                 |
| 🚶 PIR/IR Sensors      | Motion or presence detection                            |
| ⚡ Relay Module         | Switching compatible electrical loads                   |
| 💡 Light               | Controlled lighting output                              |
| 🌀 Fan                 | Controlled fan output                                   |
| 🌬️ Ventilation Device | Ventilation control, if supported by the final hardware |
| 🔋 Power Supply        | Powers the prototype                                    |
| 🧩 Breadboard          | Circuit prototyping                                     |
| 🔗 Jumper Wires        | Electrical connections                                  |

*Note: Confirm the actual sensors, output devices, and connections against the final prototype. Ventilation control requires compatible hardware and must not be claimed as a demonstrated feature unless it has been implemented.*

---

## 💻 Technologies Used

| Technology          | Application                                |
| ------------------- | ------------------------------------------ |
| 🟢 NodeMCU ESP8266  | IoT controller and connectivity            |
| ⚙️ Embedded C/C++   | Microcontroller firmware                   |
| 🐍 Python           | Backend and model development              |
| 🌐 Flask            | Backend application                        |
| 📊 Streamlit        | Monitoring dashboard                       |
| 🗄️ SQLite          | Local database                             |
| 🧠 Machine Learning | Fan/light model files and training scripts |
| 🎨 HTML             | Frontend structure                         |
| 🎨 CSS              | Frontend styling                           |
| ⚡ JavaScript        | Frontend interactions                      |
| 🛠️ Arduino IDE     | Firmware development                       |
| 🐙 Git and GitHub   | Version control and project hosting        |

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

Follow these instructions to set up the software locally.

### 📌 Prerequisites

Install the following tools:

* Python and pip
* Git
* Arduino IDE
* NodeMCU ESP8266 board support
* Required Python packages
* Required sensor and hardware libraries
* Compatible hardware for the physical demonstration

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/mahendramanikanta/Intelligent-Classroom-Monitoring-Hackathon.git
```

Navigate into the repository:

```bash
cd Intelligent-Classroom-Monitoring-Hackathon
```

### 2️⃣ Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment on Windows PowerShell:

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

### 4️⃣ Start the Flask Backend

```bash
python miniprj/backend/app.py
```

Check the terminal for the host address and port used by the application.

### 5️⃣ Launch the Streamlit Dashboard

Open a second terminal in the repository root. Activate the virtual environment if necessary, then run:

```bash
streamlit run miniprj/dashboard/dashboard.py
```

Open the local URL printed by Streamlit.

### 6️⃣ Upload the NodeMCU Firmware

1. Open the appropriate `.ino` sketch in Arduino IDE.
2. Select the NodeMCU ESP8266 board.
3. Select the correct serial/COM port.
4. Configure Wi-Fi credentials and the backend address if required.
5. Verify the sensor pin assignments.
6. Verify relay connections and output-device compatibility.
7. Upload the firmware.
8. Open Serial Monitor and check sensor readings and connection status.

⚠️ **Important:** Multiple firmware sketches are included in the repository. Select the one matching your actual hardware setup.

---

## 📊 Performance Evaluation and Results

The prototype focuses on functional monitoring and automation. The available qualitative observations cover temperature monitoring, motion detection, gas alerts, and system monitoring.

### 🧪 Functional Test Summary

| Test Parameter             | System Function                              | Qualitative Observation |
| -------------------------- | -------------------------------------------- | ----------------------- |
| 🌡️ Temperature Monitoring | Reads temperature                            | Accurate                |
| 💧 Humidity Monitoring     | Monitors humidity                            | Monitoring supported    |
| 🚶 Motion Detection        | Detects movement                             | Efficient               |
| 🌫️ Gas Detection          | Generates alerts under configured conditions | Alert generated         |
| 💡 Light Automation        | Supports lighting control                    | Automation supported    |
| 🌀 Fan Automation          | Supports fan control                         | Automation supported    |
| 📊 Dashboard Monitoring    | Displays available readings                  | Monitoring supported    |

These are qualitative observations rather than numerical benchmark results. Specific sensor accuracy, response time, or energy-consumption figures require measured test data.

---

## ⚡ Energy Efficiency and Simulated Energy Savings

Energy efficiency is an important objective of the Intelligent Classroom Monitoring and Management System.

Conventional classroom operation can leave lights and fans running when they are not required. The proposed automation approach uses environmental readings and occupancy-related sensor inputs to support more appropriate appliance operation.

Predictive fan and lighting control can be evaluated by comparing the energy consumed under a baseline operating strategy with the energy consumed under the proposed automated strategy.

Ventilation optimization can also be evaluated when the relevant control hardware and logic are available.

### 🎯 Energy-Saving Highlight

**Up to 35% simulated energy savings — target for predictive classroom appliance control.**

This figure should be reported as an achieved simulation result only if the simulation was actually run and its results support the 35% value. Otherwise, it represents a target or illustrative scenario, not a verified project outcome.

### 📐 Energy-Saving Calculation

The percentage of energy saved is calculated as:

$$
\text{Energy Savings (\%)} =
\frac{E_{\text{baseline}}-E_{\text{automated}}}
{E_{\text{baseline}}}\times100
$$

Where:

* \(E_{\text{baseline}}\) is the energy consumed under the baseline operating strategy.
* \(E_{\text{automated}}\) is the energy consumed under the automated operating strategy.

### 🧮 Illustrative 35% Energy-Saving Scenario

For example, consider a hypothetical simulation over an equivalent period:

| Parameter                          | Illustrative Value |
| ---------------------------------- | -----------------: |
| Baseline energy consumption        |           10.0 kWh |
| Energy consumption with automation |            6.5 kWh |
| Energy saved                       |            3.5 kWh |
| Percentage energy savings          |                35% |

Calculation:

$$
\text{Energy Savings} =
\frac{10.0-6.5}{10.0}\times100
=35\%
$$

This example illustrates how a 35% energy-saving result would be calculated. The values are hypothetical and must not be presented as actual simulation or hardware measurements unless supported by the project's evaluation records.

### 🔬 How the Energy-Saving Result Should Be Validated

To substantiate an energy-saving result:

1. Define the baseline strategy for operating classroom lights and fans.
2. Define the automated or predictive control strategy.
3. Use the same appliance power ratings and comparable operating periods.
4. Apply comparable occupancy and environmental conditions.
5. Calculate energy consumption for each strategy.
6. Include controller and system overhead if evaluating net energy savings.
7. Repeat the evaluation under different operating conditions.
8. Report the resulting percentage together with the test conditions.

A simulation-based result should be identified as **simulated energy savings**, while a result derived from electrical measurements should be identified as **measured energy savings**.

---

## 📈 Additional Performance Metrics

The following metrics can provide a more complete numerical evaluation.

| Metric                | Unit  | Evaluation Method                                           |
| --------------------- | ----- | ----------------------------------------------------------- |
| 🌡️ Temperature       | °C    | Compare sensor readings with a reference thermometer        |
| 💧 Humidity           | % RH  | Compare readings with a reference hygrometer                |
| ⚡ Energy Consumption  | kWh   | Calculate or measure consumption over equal periods         |
| 💡 Energy Savings     | %     | Compare baseline and automated energy consumption           |
| ⏱️ Response Time      | ms    | Measure the time between an input event and system response |
| 🎯 Detection Accuracy | %     | Compare sensor detections against verified test cases       |
| 🔌 Appliance Runtime  | Hours | Compare operating time under baseline and automated control |

No numerical accuracy or response-time results are claimed here because verified measurements have not been provided.

---

## ⚠️ Limitations

* Sensor readings depend on calibration, placement, and hardware quality.
* Automation depends on configured thresholds and implemented control logic.
* Machine-learning behavior depends on the training data, features, and model implementation.
* Gas-sensor readings are indicative and are not a substitute for certified safety equipment.
* Ventilation automation requires compatible hardware and appropriate control logic.
* The 35% energy-saving example is not a verified measurement unless supported by actual evaluation results.
* Remote access requires appropriate networking and security configuration.

---

## 🔮 Future Enhancements

* 📈 Add historical sensor-data visualization and reporting.
* ⚡ Validate energy savings through controlled simulations and real-world measurements.
* 🧠 Improve predictive control using representative classroom datasets.
* 🌬️ Integrate and evaluate automated ventilation control with compatible hardware.
* 📱 Develop a mobile-friendly monitoring interface.
* 🏫 Extend the system to multiple classrooms.
* 🔔 Add improved alert notifications.
* 🔐 Implement secure remote access and user authentication.
* 📊 Add energy-consumption reports and comparisons between operating strategies.

---

## 🎥 Project Demonstration

Want to see the physical prototype and system functionality?

▶️ **[Watch the Project Demo on Google Drive](PASTE_YOUR_GOOGLE_DRIVE_LINK_HERE)**

Make sure the video is accessible to your intended reviewers. If permitted, configure the Google Drive link so that anyone with the link can view it.

---

## 👨‍💻 Developer

**Manikanta**

🔗 GitHub: [@mahendramanikanta](https://github.com/mahendramanikanta)

---

## 🏁 Conclusion

The **Intelligent Classroom Monitoring and Management System** demonstrates the integration of IoT sensing, embedded systems, backend processing, local data storage, machine-learning components, and a monitoring dashboard.

The project explores how sensor-based monitoring and automated appliance control can contribute to more energy-conscious classroom operation.

Its energy-optimization objective includes evaluating predictive fan and lighting control, with ventilation optimization as an extension where the required hardware and logic are available.

By combining real-time sensing with automation and performance evaluation, the project provides a foundation for developing smarter classroom environments.

🚀 **Building smarter classrooms through IoT, automation, and energy-conscious technology!**

---

⭐ If you find this project interesting, consider giving the repository a star!
