## Members
Alexander Lee, Computer Engineering (2024) <br>
alexlee1017@vt.edu <br><br>

Yivvone Chen, Computer Science (2025) <br>
ychen@vt.edu

## Repo Link
<a class="button is-link" href="[https://magicmirror.builders/](https://github.com/AlexLeeVT/DancePad)" >https://github.com/AlexLeeVT/DancePad</a>

## Photo
N/A

## Mentor
N/A

## Current Status
In review

## Project Overview
Logitech Lighspeed is a technology that advertises that it's devices has less than 1ms latency while retaining a long battery life of 10-30 hours. A generic solution that can be built by the average hobbyist or student is not yet widely available. This project seeks to create an example for other projects that have use of this type of technology. The design is implemented in a dance pad as a controller on PC to show the capabilities of this technology.<br><br>

The dance pad utilizes a RP2040 as the MCU for it's relatively low power consumption and native USB support. Several peripherals are attached to provide IoT functionality and interaction with the human user. The NRF24L01+ transciever chip is used for short range low latency wireless communication between two microcontrollers and allows less than 1ms of latency. A force sensitive resistor (FSR) made with velostat and copper is utilized to provied accurate, reliable, and felxible interactions with the dance pad. It can be recalibrated to change the feeling of the pad. A battery management system is also implemented to prevent overcharging, undervolting, and power surge.

The stretch goals of this project include artistic choices and extra features. This includes adding sheet metal on top of the dance pad frame, a localally hosted website using the pi pico w's wifi compatibility to control an LED matrix, and an LED matrix to provide a lightshow while dancing.

## Educational Value Added
This project focuses on three topics: low power embedded systems, power management with LiPo batteries, and integrating electrical hardware in robust physical hardware. The students demonstrate designing low power embedded systems that utilize the nrf24L01 and LiPo batteries, applying knowledge of wireless systems (low latency short range communication, Wi-Fi, bluetooth), protyping, testing, and implementing a LiPo battery management system (BMS), desiging, testing, and validating PCBs, and practicing CAD, machining, and 3D printing skills. 

## Tasks
N/A

## Design Decisions
N/A

## Design Misc
N/A

## Steps for Documenting Your Design Process
N/A

## BOM + Component Cost
N/A

## Timeline
N/A

## Useful Links
N/A

## Log
N/A
