# CAT 9 – STM32 UART Communication

## EXPERIMENT
Continuous Lab Evaluation – 9

## DATE
[Enter Experiment Date]

## NAME OF EXPERIMENT
UART Communication

## HARDWARE SETUP / PLATFORM
- STM32 Blue Pill (STM32F103C8T6)
- USB-to-TTL Converter
- STM32CubeMX
- Keil MDK-ARM
- PuTTY
- STM32 HAL Library

## AIM
To establish serial communication between the STM32 Blue Pill and a computer using UART and implement data transmission, reception, and echo functionality.

## IMPLEMENTATION
1. Configure UART communication using STM32CubeMX.
2. Initialize UART using STM32 HAL functions.
3. Transmit messages from STM32 to the computer.
4. Receive data from the computer through UART.
5. Implement echo functionality to transmit received data back to the terminal.

## WORKING PRINCIPLE
- UART is configured for serial communication.
- STM32 transmits messages to the computer.
- Data sent from PuTTY is received by the STM32.
- The received data is transmitted back to PuTTY using echo functionality.

## CIRCUIT DIAGRAM

![UART Circuit Diagram](circuit - 1.png)

## CORE LOGIC / PSEUDOCODE
1. Initialize UART peripheral.
2. Start UART communication.
3. Transmit the required message.
4. Receive data from the serial terminal.
5. Transmit the received data back to the terminal.
6. Repeat the communication process.

## OBSERVATION
UART transmission and reception were demonstrated successfully using a serial terminal.

## INFERENCE
The experiment demonstrates UART transmission, reception, and echo communication using the STM32 Blue Pill. It provides practical understanding of serial communication and UART configuration using STM32 HAL libraries.