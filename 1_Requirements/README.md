# Wiper Control System
# Introduction
A wiper is a necessary component that cleans raindrops or any other liquid off the vehicle's windscreen. The current system required manual wiper activation,by changing the Speed frequency of wiper. As a results the operation of bringing up the wiper speed is varied . The project's goals are to improve ageing car's systems by giving automated control for wiper system, to improve the system by incorporating a sensor and actuator and to create a simple system framework. This proposed wiper system's principle is comparable to those of other existing conventional wipers. Despite the fact that. This system will be upgraded to an automatic control system using a Peripheral Interface to remove water from the windscreen.

# Software Used
STM32CubeIDE

# Components
STM32F4O7VG MICROCONTROLLER BOARD

# FEATURES OF STM32F407VG
- In a LQFP100 package, the STM32F407VGT6 microcontroller has a 32-bit ARM Cortex-M4 with FPU core, 1-Mbyte Flash memory, and 192-Kbyte RAM.

- On-board ST-LINK/V2 or ST-LINK/V2-A on STM32F4 DISCOVERY (old reference) or STM32F407G-DISC1 (new order code)

- USB ST-LINK with three separate interfaces and re-enumeration capability.

- Virtual Com port Debug port (with new order code only)

- Large-scale storage (with new order code only)

- Board power is supplied through USB or an external 5 V supply source.

- 3 V and 5 V external application power supply.

# Uses of STM32F4O7VG
- This Microcontroller is utilised in printing and scanning machines ,heat ventilation, air conditioning, and security systems.

- This module can be found in a variety of household products.

# SWOT Analysis
![image](https://user-images.githubusercontent.com/101051467/168249404-b0327752-0719-4992-a4e7-bd58063ff779.png)

## Strength:
- No need of Human Interaction.
- Viper system of Different cars can be Interfaced and handled.
- Easy handle and usage of features through a simple User Button.
- Cost efficient.
## Weakness:
- Limited usage Range.
- Less User privacy and security.
- Timers/Interrupts can be a better approach instead using Delays.
## Opportunity:
- Wide Scope in the Future of Automobiles Viper Managemnet and Control System.
- Cost efficient.
- Since advanced features can increase Car value.
## Threat:
- Now there are many new developing devices for competition in the Automobiles advancement sector.

# 4W'S and 1H

## What?
- Viper Control system where the Viper of a car is controlled by a wireless key. Viper status will be Indicated through LED's.
## WHY?
- To know the principle behind a Viper system and to manipulate its speed with respect to user's need.
## WHERE?
- Anywhere the user wants to use the feautures provided.
## WHO?
- People who are all having Car.
## HOW?
- Through a Simple and single Button.

## Requirements

# High Level Requirements
| High Level Requirements  | Description | Status |
| ----|-----------|--------------|
| HLR1  |ACC Mode Operation | Implemented |
| HLR2  | Wiper ON | Implemented |
| HLR3  | Control the speed of Wiper|Implemented |
| HLR4  |Wiper OFF|Implemented |


# Low Level Requirements
| Low Level Requirements	  | Description |Status |
| ------------- | ------------- |-----------|
| LLR1 | Pressed Button once for 2 secs| RED LED ON | Implemented |
| LLR2| Pressed Button second time|LED Blue, Green Orange blinking alternative|Implemented|
|LLR3| Pressed Button third time |LED Blue, Green, Orange blinking faster | Implemented |
|LLR4| Pressed Button fourth time |LED Blue, Green, Orange blinking fastest | Implemented |
|LLR5| Hold Button for 2 secs | Turn off all LED's|Implemented|
