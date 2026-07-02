# ICS 4111 – Embedded Systems & IoT

# Semester Project – Deliverable 2

## Group Information

| Item | Details |
|------|---------|
| Course | ICS 4111 – Embedded Systems & IoT |
| Semester | Apr – Jul 2026 |
| Deliverable | Deliverable 2 |
| Flower Assigned | Rose Plant |
| Repository | https://github.com/Codex-r1/Ctrl-Alt-Elite-/ |

---

# 1. Introduction

This deliverable focuses on the implementation of embedded system prototypes based on the architectures proposed in Deliverable 1. Both physical and simulated prototypes were developed using ESP32S microcontrollers together with environmental sensors used for monitoring rose plant growth.

The prototypes demonstrate successful acquisition of environmental data, communication between embedded devices, and display of sensor readings through an OLED display and Serial Monitor.

---

# 2. Prototype Summary

| Architecture | Physical Prototype | Simulated Prototype |
|--------------|-------------------|---------------------|
| Architecture A | ✓ | ✓ |
| Architecture B | ✓ | ✗ |
| Architecture C | ✗ | ✓ |

A total of four prototypes were successfully developed as required:

- Physical Prototype A
- Simulated Prototype A
- Physical Prototype B
- Simulated Prototype C

---

# 3. Prototype A

## ESP32S Connected to DHT22, MQ-5 and OLED Display

## Objective

To monitor temperature, humidity and gas concentration using a single ESP32S and display sensor readings on an OLED display.

---

## Components Used

- ESP32S Development Board
- DHT22 Temperature and Humidity Sensor
- MQ-5 Gas Sensor
- 128×64 OLED Display
- 10kΩ Pull-up Resistor
- Breadboard
- Jumper Wires
- USB Cable

---

## Physical Prototype

### Circuit

> Insert image of the assembled physical prototype.

![Physical Prototype A](images/prototypeA.jpg)

---

### OLED Display Output

> Insert image showing OLED displaying readings.

![OLED Output](images/prototypeA_oled.jpg)

---

### Serial Monitor Output

> Insert screenshot of Arduino IDE Serial Monitor.

![Serial Monitor](images/prototypeA_serial.png)

---

## Simulation

### Wokwi Project

Replace with your actual public Wokwi link.

https://wokwi.com/projects/XXXXXXXXXXXX

---

### Simulation Screenshot

![Simulation A](images/wokwiA.png)

---

## Results

The ESP32 successfully:

- Read temperature from the DHT22 sensor.
- Read humidity from the DHT22 sensor.
- Read gas concentration from the MQ-5 sensor.
- Displayed all readings on the OLED display.
- Printed real-time readings to the Serial Monitor.

---

# 4. Prototype B

## ESP32S Connected to MQ-5 Interfaced Directly with Another ESP32S Connected to DHT22

## Objective

To demonstrate communication between two ESP32 microcontrollers where one node acquires gas data while the second node acquires environmental data.

---

## Components Used

- ESP32S (2)
- MQ-5 Sensor
- DHT22 Sensor
- Breadboard
- Jumper Wires
- USB Cables

---

## Physical Prototype

### Circuit

Insert image.

![Prototype B](images/prototypeB.jpg)

---

### Serial Monitor Output (ESP32 Node 1)

Insert screenshot.

![Node1](images/node1_serial.png)

---

### Serial Monitor Output (ESP32 Node 2)

Insert screenshot.

![Node2](images/node2_serial.png)

---

## Communication

The two ESP32 boards communicate directly to exchange sensor readings.

Data transmitted includes:

- Temperature
- Humidity
- Gas concentration

---

## Results

The prototype successfully demonstrated communication between two ESP32 development boards while collecting environmental sensor data.

---

# 5. Prototype C

## ESP32S Connected to DHT22 Connected Through Relay to Another ESP32S Connected to MQ-5

## Objective

To demonstrate relay-based interaction between two embedded subsystems.

---

## Components Used

- ESP32S (2)
- Relay Module
- MQ-5 Sensor
- DHT22 Sensor
- Breadboard
- Jumper Wires

---

## Simulation

### Wokwi Project

Replace with your public link.

https://wokwi.com/projects/YYYYYYYYYYYY

---

### Simulation Screenshot

![Simulation C](images/wokwiC.png)

---

## Output

The simulation demonstrated:

- Successful DHT22 readings.
- Relay activation.
- Communication with second ESP32.
- MQ-5 sensor monitoring.

---

# 6. Software Development

## Development Environment

- Arduino IDE
- ESP32 Board Package
- Wokwi IoT Simulator

---

## Libraries Used

- DHT Sensor Library
- Adafruit Unified Sensor Library
- Adafruit SSD1306
- Adafruit GFX Library
- Wire Library

---

# 7. Challenges Encountered

| Challenge | Solution |
|------------|----------|
| Incorrect sensor readings | Checked wiring connections and GPIO assignments. |
| OLED display not detected | Verified I2C address and SDA/SCL pins. |
| MQ-5 unstable readings | Allowed adequate sensor warm-up time before recording values. |
| ESP32 communication delays | Improved timing logic and verified serial communication settings. |

---

# 8. Evidence of Group Work

## Prototype Development

Insert images showing group members assembling the hardware.

![Group Work](images/groupwork1.jpg)

---

## Testing Session

Insert image.

![Testing](images/groupwork2.jpg)

---

## Team Discussion

Insert screenshot of meeting or communication.

![Meeting](images/meeting.png)

---

## Task Allocation

| Team Member | Responsibility |
|------------|----------------|
| Phillip Gakuo | Prototype assembly |
| Abucheli Ronah | Hardware integration and testing |
| Danny Podho | Software development |
| Phillip Leo | Wokwi simulations |
| Njihia Muranga | Documentation and GitHub repository management |

---

# 9. Discussion

The developed prototypes successfully demonstrated the implementation of embedded IoT architectures proposed during Deliverable 1.

Both physical and simulated systems were capable of acquiring environmental data relevant to rose plant growth. Sensor readings were displayed locally using an OLED display and monitored through the Arduino IDE Serial Monitor. The distributed architectures further demonstrated communication between multiple ESP32 microcontrollers, illustrating how environmental monitoring tasks can be shared among embedded nodes.

The prototypes provide a solid foundation for the final integrated smart rose plant monitoring system.

---

# 10. Conclusion

The objectives of Deliverable 2 were successfully achieved through the implementation of both physical and simulated embedded system prototypes. Four working prototypes were produced in accordance with the project requirements. The systems successfully monitored environmental parameters and demonstrated communication between embedded devices. These prototypes will serve as the basis for future IoT integration and cloud connectivity in subsequent project deliverables.

---

