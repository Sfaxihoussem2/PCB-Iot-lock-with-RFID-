# Pointeuse IoT Lock - RFID-Based PCB Design

This repository contains the PCB design and schematic files for an **IoT-based lock system using RFID technology**. The project, named **Pointeuse IoT Lock**, is designed to provide secure access control using RFID cards or tags, integrated with IoT capabilities for remote monitoring and management.

---

## Project Overview

The Pointeuse IoT Lock system is a secure access control solution that uses RFID technology to authenticate users. The system is designed to be integrated with IoT platforms for remote access management, real-time monitoring, and logging of access events.

### Key Features:
- **RFID Authentication**: Users can unlock the system using RFID cards or tags.
- **IoT Integration**: The system can be connected to an IoT platform for remote monitoring and control.
- **Secure Access**: Only authorized RFID tags are granted access.
- **Real-Time Logging**: Access events are logged and can be monitored remotely.
- **Buzzer and LED Indicators**: Provides audio and visual feedback for access granted/denied.

---

## Repository Contents

### 1. **Schematic Files**
  ![Schematic_pointeuse](Schematic2.png)
   - **Schematic**
     - Contains the schematic diagram for the Pointeuse IoT Lock system.
     - Includes components such as resistors, DC components, and RFID module connections.
 ![Schematic_pointeuse](Schematic.png)   
   - **Schematic**
     - Contains a schematic for a related project with detailed component connections.

### 2. **PCB Design Files**
   ![PCB](PCB.png)
   - **PCB**
     - Contains the PCB layout for the Pointeuse IoT Lock system.
     - Includes components such as U1 (microcontroller), resistors (R1, R2), and transistors (Q4, Q5, Q6).
    ![PCB](PCB2.png)
   - **PCB*
     - Contains the PCB layout for a related project with components like RDM63001, antennas (ANT1, ANT2), LEDs, and a buzzer.

---

## Components Used

### Main Components:
- **RFID Module**: For reading RFID cards/tags.
- **Microcontroller (U1)**: Acts as the brain of the system, processing RFID data and controlling access.
- **Antennas (ANT1, ANT2)**: Used for RFID signal transmission and reception.
- **Resistors (R1, R2)**: For current regulation and signal conditioning.
- **Transistors (Q4, Q5, Q6)**: For switching and control logic.
- **LEDs (LED1, LED2)**: For visual feedback (e.g., access granted/denied).
- **Buzzer (BUZZER1)**: For audio feedback (e.g., access granted/denied).
- **Connectors (RX, TX, +5V, GND)**: For communication and power supply.

### Additional Components:
- DC components (DC1 to DC730) for power management and signal routing.
- Various resistors, capacitors, and transistors for circuit stability.

---

## How It Works

1. **RFID Authentication**:
   - When an RFID card/tag is presented to the reader, the RFID module reads the unique ID.
   - The microcontroller verifies the ID against a pre-authorized list.
   - If the ID is valid, access is granted, and the lock is opened.

2. **IoT Integration**:
   - The system can be connected to an IoT platform (e.g., MQTT, AWS IoT, or Blynk) for remote monitoring.
   - Access events (granted/denied) are logged and sent to the IoT platform.
   - Administrators can manage access permissions remotely.

3. **Feedback**:
   - **LEDs**: Indicate access status (e.g., green for granted, red for denied).
   - **Buzzer**: Provides an audible alert for access events.

---

## Usage

### Steps to Use the PCB Design:
1. **Download the Files**:
   - Download the schematic and PCB design files from this repository.
2. **Open in PCB Design Software**:
   - Use software like KiCad, Eagle, or Altium to open and modify the files.
3. **Fabricate the PCB**:
   - Export the PCB design and send it to a PCB manufacturer for fabrication.
4. **Assemble the Components**:
   - Solder the components onto the PCB as per the schematic.
5. **Upload Firmware**:
   - Program the microcontroller with the appropriate firmware for RFID and IoT functionality.
6. **Test the System**:
   - Test the system with RFID cards/tags and ensure proper integration with the IoT platform.

---

## License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute the files for personal or commercial use. See the [LICENSE](LICENSE) file for more details.
