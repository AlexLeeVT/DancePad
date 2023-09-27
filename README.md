## Members
Alex Lee, Computer Engineering (2024) <br>
alexlee1017@vt.edu <br><br>

Yvvy Chen, Computer Science (2025) <br>
yvvyc@vt.edu

## Repo Link
<a class="button is-link" href="[https://magicmirror.builders/](https://github.com/AlexLeeVT/DancePad)" >https://github.com/AlexLeeVT/DancePad</a>

## Photo
N/A

## Mentor
Neil B.

## Current Status
Approved/In Developent

## Project Overview
Logitech Lightspeed is a technology that advertises that it's devices has less than 1ms latency while retaining a long battery life of 10-30 hours. A generic solution that can be built by the average hobbyist or student is not yet widely available. This project seeks to create an example for other projects that have use of this type of technology. The design is implemented in a dance pad as a controller on PC to show the capabilities of this technology.<br><br>

The dance pad utilizes a RP2040 as the MCU for it's relatively low power consumption and native USB support. Several peripherals are attached to provide IoT functionality and interaction with the human user. The NRF24L01+ transciever chip is used for short range low latency wireless communication between two microcontrollers and allows less than 1ms of latency. A force sensitive resistor (FSR) made with velostat and copper is utilized to provied accurate, reliable, and felxible interactions with the dance pad. It can be recalibrated to change the feeling of the pad. A LiPo battery is used for wireless functionality and its battery management system is also implemented to prevent overcharging, undervolting, and power surge.<br><br>

The stretch goals of this project include artistic choices and extra features. This includes adding sheet metal on top of the dance pad frame, a localally hosted website using the pi pico w's wifi compatibility to control an LED matrix and configure many onboard features of the system, and an LED matrix to provide a lightshow while dancing.

## Educational Value Added
This project focuses on three topics: low power embedded systems, power management with LiPo batteries, and integrating electrical hardware in robust physical hardware. The students demonstrate designing low power embedded systems that utilize the nrf24L01 and LiPo batteries, applying knowledge of wireless systems (low latency short range communication, Wi-Fi, bluetooth), implementing an IoT protocol, protyping, testing, and implementing a LiPo battery management system (BMS), desiging, testing, validating PCBs, practicing CAD, machining, and 3D printing skills, and learning safety for machining parts and in managing LiPo batteries. 

## Tasks
N/A

## Design Decisions
   The purpose of this project is to create a wireless low power embedded system with short range wireless communication that has low latency between the transmitter and receiver. For this purpose, two microcontrollers are utilized: esp32 and pi pico. The Pi Pico has a simple to implement design with a low cost of $5 per module. It is also compatible with TUSB, a library that interfaces with the USB protocol on Windows. It allows the Pi Pico to function as a keyboard, gamepad, or even a MIDI device but for the purpose of this project, it will only act as a gamepad. The pi pico has two wireless protocols on board: bluetooth and wifi, however both are costly in terms of power consumption and latency. It also might have interference from other local devices with the same protocols attempting to connect to the networks. Their purpose, while can be used for data transfer, is not meant strictly for peer to peer connections -- rather it is for a more general applications. Instead of using WiFi, Bluetooth, or LoRa, the NRF24l01 transciever (configured as a receiver) is utilized as the wireless communication module to communicate between the ESP32 (which also has ble and WiFi) and Pi Pico. 
   The ESP32 is utilized for it's versatility in functionality and IO ports and is used as the microcontroller on the wireless system. It has built in low power functionality with 20 ADC pins available which will be important in a later design point. The low power funcionality disables unnecessary modules that consume power such as the BLE and WiFi modules meaning a lower average power consumption is observed. When power efficiency is important, any features that lower power consumption are important. Other modules found on the system are force sensitive resistors (FSRs), the NRF24l01 configured as the transmitter, and BMS and protection circuit for the LiPo battery.
   Physical hardware is important for human interaction with the device. Structural integrity is an integral feature of the system as high impact force is often observed

## Design Misc
N/A

## Steps for Documenting Your Design Process
during design and development, record short videos documenting the process and reporting progress on the project.

## BOM + Component Cost

Pi Pico - $5
ESP32 - $30
LiPo battery - ~$10
PCB & components - ~$2-5
velostat - $5
copper ribbon
plywood/osb - ~$20
MDF - $43
screws - $12
polycarbonate - $88

## Timeline
1. Prototype and develop electronics
   - force sensitive resistors & LiPo battery charger must function
   - low power functionality with the microcontroller must be achieved
   - PCB constructed, but does not have to be finalized.
2. Construct and build frame for the DDR/PIU dance pad
   - 3D CAD file constructed
   - MDF base must have FSRs installed and polycarbonate panels with spacers must be completed
3. Finishing touches and wireless connectivity
   - ~3-5ms wireless latency with <1ms USB latency with PC

## Useful Links
GreatScott! single cell lipo battery charger - [https://www.youtube.com/watch?v=6LxRnf6sQNQ](https://www.youtube.com/watch?v=6LxRnf6sQNQ)

## Log
N/A
