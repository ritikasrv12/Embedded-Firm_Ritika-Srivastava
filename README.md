# Smart Water Heater and AC Load Bank Assignment

## Submitted by
*Name:* Ritika Srivastava  
*Registration Number:* 21BEC10011  

---

## Part 1: Smart Water Heater

### Objective
To design a smart water heater system integrating energy efficiency, precise measurement, safety mechanisms, and remote operability.

### Key Components
1. *Hardware Design*
   - *Sensors:*
     - Temperature Sensor (DS18B20/PT100) for water temperature.
     - Water Level Sensor (Ultrasonic/Float) for monitoring water level.
   - *Microcontroller:*
     - ESP32 for data processing and Wi-Fi communication.
   - *Actuators:*
     - Heating Element for temperature regulation.
     - Valves for water flow control.
   - *Power Supply:*
     - AC-DC Converter, Relay Module, and Circuit Breaker.

2. *Firmware Design*
   - Data Processing, PID Algorithm, Safety Logic, and Wi-Fi communication.

3. *Software Design*
   - *User Interfaces:*
     - Mobile App and Web Dashboard for system interaction.
   - *Cloud Connectivity:*
     - API Gateway and Cloud Database for data storage and analysis.
   - *Backend Modules:*
     - Control Module, Data Processing, Diagnostics, and Analytics.

### Features
- Remote monitoring and control.
- Energy efficiency via PID Algorithm.
- Safety mechanisms like overheat protection.

---

## Part 2: AC Load Bank

### Objective
To design a program to control an AC load bank for achieving specific load setpoints via relays.

### System Overview
- *Load Steps:* 100W, 200W, 500W, 1000W, 2000W, 3000W, and 5000W.
- *Relay Control Logic:*
  - Greedy algorithm to activate minimum relays.
  - Error handling for unachievable setpoints.

### Key Features
1. *Input Handling:* Validates load setpoints via UART communication.
2. *Relay Control:* Prioritizes larger load steps to minimize relay usage.
3. *Communication:* Sends relay states via UART.
4. *Visualization:* Displays relay states (ON/OFF) and corresponding load steps.

### Workflow
1. Receive load setpoint via UART.
2. Validate input.
3. Calculate relay states using a greedy algorithm.
4. Send states via UART.
5. Visualize relay states.
6. Handle unachievable setpoints with error messages.

### Example
- *Input Setpoint:* 3200W
- *Activated Relays:* 3000W (Relay 2) and 200W (Relay 9)
- *Visualization:* Green rectangles for active relays, gray for inactive.

---

## Implementation
The project includes both hardware and software design diagrams, along with Python code for the AC Load Bank program.

### Code for AC Load Bank
Refer to the assignment document for detailed Python code implementation.

---

## Conclusion
This assignment demonstrates the integration of hardware, firmware, and software components in the smart water heater project, alongside an efficient relay-based control system for the AC load bank.
