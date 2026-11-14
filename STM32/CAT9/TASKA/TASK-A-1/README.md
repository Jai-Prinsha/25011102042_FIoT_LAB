# CAT 9 (A1) – UART Data Transmission

## EXPERIMENT

Continuous Lab Evaluation – 9

## DATE

[Enter Experiment Date]

## NAME OF EXPERIMENT

UART Data Transmission

## HARDWARE SETUP / PLATFORM

- STM32 Blue Pill (STM32F103C8T6)
- USB-to-TTL Converter
- STM32CubeMX
- Keil MDK-ARM
- PuTTY
- STM32 HAL Library

## AIM

To establish UART communication between the STM32 Blue Pill and a computer and transmit messages through a serial terminal.

## IMPLEMENTATION

1. Configure UART communication using STM32CubeMX.
2. Initialize UART using STM32 HAL functions.
3. Transmit messages from the STM32 to the computer.
4. Display the transmitted messages using PuTTY.

## WORKING PRINCIPLE

- UART is configured for serial communication.
- STM32 initializes the UART peripheral.
- Messages are transmitted from STM32 to the computer.
- PuTTY displays the received messages.

## CIRCUIT DIAGRAM

![UART Circuit Diagram](circuit.png)

## CORE LOGIC / PSEUDOCODE

1. Initialize the UART peripheral.
2. Start UART communication.
3. Prepare the message to be transmitted.
4. Transmit the message to the computer.
5. Display the message in PuTTY.
6. Repeat the transmission process.

## OBSERVATION

UART message transmission from STM32 to the computer was demonstrated successfully using a serial terminal.

## INFERENCE

The experiment demonstrates UART initialization and serial data transmission using the STM32 Blue Pill and STM32 HAL libraries.