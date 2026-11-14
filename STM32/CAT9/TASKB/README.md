# CAT 9 – UART-Based LED Control

## EXPERIMENT
Continuous Lab Evaluation – 9

## NAME OF EXPERIMENT
String-Based LED Control Using UART

## HARDWARE SETUP / PLATFORM
- STM32 Blue Pill (STM32F103C8T6)
- USB-to-TTL Converter
- LED (PC13)
- STM32CubeMX
- Keil MDK-ARM
- PuTTY
- STM32 HAL Library

## AIM
To control an LED connected to PC13 of the STM32 Blue Pill using string commands received through UART communication.

## IMPLEMENTATION
1. Receive command data through UART.
2. Process the received string.
3. Identify the received command.
4. Control the LED connected to PC13 based on the received command.

## WORKING PRINCIPLE
- UART receives command data from the computer.
- The STM32 processes the received string.
- The received command is identified.
- Based on the command, the LED connected to PC13 is controlled.

## Circuit Diagram
![UART and LED Circuit Diagram](../../circuit - 2.png)


## CORE LOGIC / PSEUDOCODE
1. Initialize GPIO and UART peripherals.
2. Start UART communication.
3. Receive command data from the serial terminal.
4. Process the received string.
5. Compare the received command.
6. Control the PC13 LED according to the command.
7. Repeat the communication process.

## OBSERVATION
The LED responded to the commands received through the serial terminal.

## INFERENCE
The experiment demonstrates UART-based string command processing and GPIO control using the STM32 Blue Pill. It provides practical understanding of serial communication and command-based LED control using STM32 HAL libraries.