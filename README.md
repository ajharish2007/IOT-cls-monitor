# 🏠 IoT Home Automation System using ESP32 and Firebase

## 📌 Project Overview

This project demonstrates an **IoT-based Home Automation System** using an ESP32 microcontroller, sensors, Firebase Realtime Database, and a web dashboard.

The system collects sensor data, sends it to Firebase through Wi-Fi, and allows users to monitor the data remotely using a web browser on a computer or mobile phone.

The hardware is simulated using **Wokwi**, making it possible to develop and test the project without physical components.


## 🎯 Objectives

* Develop a simple IoT-based home automation system.
* Interface sensors with the ESP32 microcontroller.
* Send sensor data to Firebase Realtime Database.
* Display real-time data on a web dashboard.
* Enable remote monitoring through a mobile-friendly website.
* Simulate and test the hardware using Wokwi.

## 🛠️ Technologies Used

| Technology                 | Purpose                    |
| -------------------------- | -------------------------- |
| ESP32                      | Microcontroller            |
| C++ (Arduino)              | Embedded programming       |
| Wokwi                      | Hardware simulation        |
| Wi-Fi                      | Internet connectivity      |
| Firebase Realtime Database | Cloud data storage         |
| HTML                       | Dashboard structure        |
| CSS                        | Dashboard design           |
| JavaScript                 | Real-time database updates |
| Firebase Hosting           | Website deployment         |

## 🏗️ System Architecture

```text
Sensors
   |
   v
ESP32 Microcontroller
   |
   v
Wi-Fi Connection
   |
   v
Firebase Realtime Database
   |
   v
Web Dashboard
   |
   v
Mobile Phone / Computer
```

## ⚙️ Working Principle

1. Sensors collect information from the home environment.
2. The ESP32 reads sensor values and processes the data.
3. The ESP32 connects to Wi-Fi.
4. Sensor readings are sent to Firebase Realtime Database.
5. The web dashboard retrieves updates from Firebase.
6. Users can monitor the current sensor readings from their mobile phone or computer.
7. Based on programmed conditions, the ESP32 can control connected output devices such as a fan or LED.

## 🔌 Hardware Components

* ESP32 development board
* Two sensors suitable for the selected automation functions
* LED or relay module for output control
* Breadboard and jumper wires (for physical implementation)

**Note:** The components and connections depend on the specific sensors selected for the project. Wokwi is used for simulation.

## ☁️ Firebase Integration

Firebase Realtime Database stores the sensor readings in the cloud. The ESP32 sends data over HTTPS, and the dashboard listens for database changes to display updated values.

Example database structure:

```json
{
  "home": {
    "temperature": 28,
    "motionDetected": false,
    "fanStatus": "OFF"
  }
}
```

*The values above are illustrative examples; the actual structure depends on the implemented sensors and code.*

## 🌐 Web Dashboard

The dashboard provides a simple interface to:

* View current sensor readings.
* Monitor connected device status.
* Receive real-time updates from Firebase.
* Access the monitoring page from a mobile phone or computer after deployment.

## 🚀 How to Run the Project

### 1. Simulate the hardware

1. Open your Wokwi ESP32 project.
2. Add the selected sensors and output components.
3. Connect the components according to the Arduino code.
4. Start the simulation.

### 2. Configure Firebase

1. Create a project in the [Firebase Console](https://console.firebase.google.com/).
2. Enable Realtime Database.
3. Copy the database URL.
4. Configure the ESP32 code and web dashboard with the appropriate Firebase details.
5. Set up appropriate database security rules.

### 3. Run the web dashboard locally

1. Open the dashboard folder in Visual Studio Code.
2. Open `index.html` using the Live Server extension.
3. Confirm that the dashboard connects to Firebase.
4. Verify that new database values appear on the page.

### 4. Deploy the dashboard

1. Install Node.js and Firebase CLI.
2. Sign in to Firebase using the CLI.
3. Initialize Firebase Hosting in the website folder.
4. Deploy the website.
5. Open the generated public URL on a mobile phone or computer.

See the [Firebase Hosting documentation](https://firebase.google.com/docs/hosting) for detailed deployment instructions.

## 🔒 Security Considerations

* Do not commit passwords, private keys, or service-account credentials to GitHub.
* Configure Firebase Authentication and appropriate Realtime Database security rules.
* Avoid unrestricted public database read/write access.
* Use secure certificate validation in production firmware.
* Restrict access to authorized users.

## 🔮 Future Enhancements

* Add temperature and humidity monitoring.
* Add motion detection for automatic lighting.
* Control appliances through a mobile-friendly dashboard.
* Add alerts when sensor values exceed defined limits.
* Add user authentication.
* Improve energy monitoring and automation logic.
* Integrate additional IoT sensors.

## 📚 Applications

* Smart homes
* Remote environmental monitoring
* Energy-efficient automation
* IoT learning and prototyping
* Smart building applications

## 👨‍💻 Project Status

**Development and simulation:** In progress.

The project uses Wokwi for hardware simulation, Firebase for cloud storage, and a web dashboard for remote monitoring. Final features depend on the sensors and control logic implemented.

## 📄 License

This project is intended for educational and learning purposes. Add a license file to specify how others may use, modify, and distribute the code.
**SIMULATION**:https://wokwi.com/projects/477393567216978945

