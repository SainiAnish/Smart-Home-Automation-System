# Smart-Home-Automation-System
1. Project Overview

A complete IoT-based Smart Home Automation system that allows users to monitor and control home appliances and safety systems remotely via the Blynk IoT platform.
It integrates sensors, actuators, and automation logic to improve convenience, safety, and energy efficiency.

2. Key Components & Their Functions

Device/Component	Function

ESP8266 NodeMCU	Main controller; connects devices to Wi-Fi and Blynk cloud.

Blynk IoT Platform	Mobile/web dashboard for remote monitoring and control.

DHT22 Sensor	Measures temperature and humidity.

PIR Motion Sensor	Detects human movement for security & auto-lighting.

MQ-2 Gas Sensor	Detects flammable gases (LPG, methane) and smoke.

Flame Sensor	Detects fire or open flame presence.

Water Leak Sensors	Detects water leaks in kitchen/bathroom.

Relays (5-channel)	Switch AC appliances (lights, fan, pump, siren) ON/OFF.

Servo Motor	Controls door lock position (locked/unlocked).

Buzzer/Siren	Sounds alarm during fire, gas leak, or water leak.

3. Implementation Steps

Hardware Setup :
Connect sensors and actuators to ESP8266 GPIO pins.

Use relay modules for controlling AC appliances.

Power and connect all components to common ground.


Software Setup  :
Install Arduino IDE with ESP8266 board support.

Install Blynk, DHT, and Servo libraries.

Load the provided Arduino sketch with your Wi-Fi credentials & Blynk token.


Blynk Dashboard  :
Create widgets (switches, sliders, time inputs, value displays).

Map each widget to its respective virtual pin (V0–V18).

Create event alerts for gas leak, fire, and water leak.


Automation Rules :
Motion-based lighting at night (via time window).

Auto-fan when temperature exceeds threshold.

Automatic siren and alert notifications for safety events.



4. How It Works

Sensing: DHT22, PIR, MQ-2, flame, and water leak sensors detect environmental changes.

Processing: ESP8266 processes sensor data and checks automation rules.

Actuation: Relays control appliances; servo operates the door lock.

Communication: ESP8266 sends data to Blynk cloud over Wi-Fi.

Control: User can operate devices manually via app or let automation handle them.

Alerts: Gas/fire/leak events trigger the siren and send instant notifications.



5. Benefits

Remote access & control from anywhere.

Energy efficiency through automated fan & light control.

Enhanced safety with fire, gas, and water leak detection.

Customizable time windows, thresholds, and automation rules.

Scalable — more sensors/appliances can be added easily.


Enhanced safety with fire, gas, and water leak detection.

Customizable time windows, thresholds, and automation rules.

Scalable — more sensors/appliances can be added easily.
