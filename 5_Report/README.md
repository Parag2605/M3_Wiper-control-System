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

# Requirements

## High Level Requirements
| High Level Requirements  | Description | Status |
| ----|-----------|--------------|
| HLR1  |ACC Mode Operation | Implemented |
| HLR2  | Wiper ON | Implemented |
| HLR3  | Control the speed of Wiper|Implemented |
| HLR4  |Wiper OFF|Implemented |


## Low Level Requirements
| Low Level Requirements	  | Description |Status |
| ------------- | ------------- |-----------|
| LLR1 | Pressed Button once for 2 secs| RED LED ON | Implemented |
| LLR2| Pressed Button second time|LED Blue, Green Orange blinking alternative|Implemented|
|LLR3| Pressed Button third time |LED Blue, Green, Orange blinking faster | Implemented |
|LLR4| Pressed Button fourth time |LED Blue, Green, Orange blinking fastest | Implemented |
|LLR5| Hold Button for 2 secs | Turn off all LED's|Implemented|

# Architecture
## Block Diagram
![Block Diagram](https://user-images.githubusercontent.com/101051467/168366499-5ac4222d-88a2-40ea-9703-48f82075c286.PNG)

## Flow Chart
![Flow Chart](https://user-images.githubusercontent.com/101051467/168366982-ce623f07-dbda-4557-b156-6b48720d12c8.png)

## UML
![UML](https://user-images.githubusercontent.com/101051467/168370857-747bbbcd-70bc-4d27-90a7-c63c46fdfca5.png)

# TestPlanAndOutput
## HIGH LEVEL TEST PLAN

| Test ID | Description | Input | Expected output | Actual Output | 
| --- | --- | --- | --- | --- | 
| 01 | Ignition On | 1st 2sec User Button Press | Ignition key status | Displayed Ignition key status  | 
| 02 | Viper On | 1st User Button Press | Viper Status-1Hz | Displayed Viper Status | 
| 03 | Viper On | 2nd User Button Press | Viper Status-4Hz | Displayed Viper Status | 
| 04 | Viper On | 3rd User Button Press | Viper Status-8Hz | Displayed Viper Status | 
| 05 | Ignition Off | 2nd 2sec User Button Press |  Ignition key status  | Displayed Ignition key status  | 

### Here below are the some of the *unity test/ unity framework* test plans there are so many but I have only mentiones some of the test cases here.

## LOW LEVEL TEST PLAN

| Test ID | Description | Input | Expected output | Actual Output | Passed Or Not |
| --- | --- | --- | --- | --- | --- |

| Test ID (for LED)| Description | Input | Expected output | Actual Output | passed/not |
| --- | --- | --- | --- | --- | --- |
| 01 | Check for ignition_on() | 1st 2sec User Button Press | RED LED ON | RED LED ON | ✅ |
| 02 | Check for led_cycle1() | 1st User Button Press | All LEDs ON | All LEDs ON-1Hz | ✅ |
| 03 | Check for led_cycle1() | 1st User Button Press | All LEDs ON | All LEDs ON-4Hz| ✅ |
| 04 | Check for led_cycle1() | 1st User Button Press | All LEDs ON | All LEDs ON-8Hz | ✅ |
| 04 | Check for ignition_off() | 2nd 2sec User Button Press | RED LED OFF | RED LED OFF | ✅ |

| Test ID (for Button Count For Turning Viper on)| Description | Input | Expected output | Actual Output | passed/not |
| --- | --- | --- | --- | --- | --- |
| 01 | Check for Button_Count() | 1 User Button Press | 1 | 1 | ✅ |
| 02 | Check for Button_Count() | 2 User Button Presses | 2 | 2 | ✅ |
| 03 | Check for Button_Count() | 3 User Button Presses | 3 | 3 | ✅ |

---

# Output
## Blinking three LED
![image](https://user-images.githubusercontent.com/101051467/168275285-f1313b6d-df4d-4ce5-8e70-5f44d35183a1.png)

## Press Button once for 2 sec
![image](https://user-images.githubusercontent.com/101051467/168275380-1409629d-bd27-45e4-bf68-c87fb886f4a5.png)

## Wiper ON
![image](https://user-images.githubusercontent.com/101051467/168276126-f64e715c-7348-4c9a-a8f8-8275a513d349.png)

## Wiper Speed Change
![image](https://user-images.githubusercontent.com/101051467/168276204-996588a3-64c5-48bd-8884-c735382b2e55.png)

## Press Button again for 2 sec
![image](https://user-images.githubusercontent.com/101051467/168276503-b2d0c0ff-3f13-4dfd-b106-781464aebdf2.png)

## Video
https://user-images.githubusercontent.com/101051467/168486398-a7bc8f3b-0938-4c12-bb09-41606ceb38ab.mp4
