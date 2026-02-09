# Bluetooth Controlled RC Car Using ESP32

A remote-controlled car powered by ESP32, capable of moving forward, backward, left, and right using Bluetooth commands. This project demonstrates wireless motor control and basic robotics principles.

---

## Introduction
This project focuses on the design and development of a Bluetooth-controlled RC car using the ESP32 microcontroller. The main objective is to demonstrate wireless control of a robotic vehicle using a smartphone or Bluetooth-enabled device. By integrating a motor driver and Bluetooth communication, the RC car can receive commands in real time.

The project helps in understanding the fundamentals of embedded systems, motor control, and sensor interfacing. Such systems can be applied in robotics education, hobbyist projects, and small autonomous vehicles.

---

## Components Used

| Component | Description | Purpose |
|-----------|------------|--------|
| 4-Wheel Chassis | Mechanical base with wheels | Provides structure and movement |
| BO Motors (4) | DC geared motors | Drive the wheels |
| ESP32 | Microcontroller with Wi-Fi & Bluetooth | Main controller |
| Motor Driver | L298N Dual H-Bridge | Controls motor direction and speed |
| Ultrasonic Sensor | HC-SR04 | Detect obstacles (optional) |
| Jumper Wires | Male-to-Male / Male-to-Female | Electrical connections |
| Batteries | Li-ion / AA | Power supply |
| Battery Holders | Secure battery placement | Power management |
| Buzzer | Piezo buzzer | Audio alert |
| Resistors | Various values | Current limiting |
| LEDs | Indicator LEDs | Status indication |

---

## System Diagrams

### Block Diagram
![Block Diagram](images/block_diagram.png)  
*The ESP32 receives Bluetooth commands from a smartphone and controls the motor driver to move the car. LEDs and buzzer provide status alerts.*

### Circuit Diagram
![Circuit Diagram](images/circuit_diagram.png)  
*The ESP32 GPIO pins are connected to the L298N motor driver and sensors. Power is supplied separately to ensure stable operation.*

---

## Problems Faced
- Voltage drop issues when motors drew high current  
- Motor noise caused unstable movement  
- Bluetooth connection delays  
- Limited current capacity of L298N driver  
- Proper pin selection on ESP32 due to GPIO restrictions  
- Loose jumper wire connections during testing  

---

## Future Improvements
- Replace HC-06 with ESP32 native Bluetooth for better performance  
- Use a more efficient motor driver such as TB6612FNG  
- Add PWM-based speed control  
- Integrate obstacle detection using ultrasonic sensors  
- Enable Wi-Fi or mobile app control  
- Add camera or additional sensors for advanced features  

---

## Conclusion
The Bluetooth-controlled RC car project successfully demonstrates wireless control of a robotic vehicle using the ESP32. The project provided hands-on experience with motor drivers, Bluetooth communication, and embedded programming. Despite minor hardware and power challenges, the system performed as expected and lays the foundation for more advanced robotics projects.

---

## Images
*(Replace the placeholders with your actual images)*  
![RC Car Prototype](images/rc_car_front.png)  
![RC Car Top View](images/rc_car_top.png)
