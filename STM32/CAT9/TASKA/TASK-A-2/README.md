# CAT 9 (A2) – UART Data Reception and Echo

## EXPERIMENT

Continuous Lab Evaluation – 9


## NAME OF EXPERIMENT

UART Data Reception and Echo

## HARDWARE SETUP / PLATFORM

- STM32 Blue Pill (STM32F103C8T6)
- USB-to-TTL Converter
- STM32CubeMX
- Keil MDK-ARM
- PuTTY
- STM32 HAL Library

## AIM

To receive data from a computer through UART communication and transmit the received data back to the computer using echo functionality.

## IMPLEMENTATION

1. Configure UART communication using STM32CubeMX.
2. Initialize UART using STM32 HAL functions.
3. Receive data from the computer through UART.
4. Transmit the received data back to the terminal.
5. Implement echo functionality.

## WORKING PRINCIPLE

- UART is configured for serial communication.
- Data entered in PuTTY is received by the STM32.
- STM32 reads the received data through UART.
- The received data is transmitted back to PuTTY.
- The terminal displays the echoed data.

## Circuit Diagram
Refer to the parent Task A README for the circuit diagram

## CORE LOGIC / PSEUDOCODE

1. Initialize the UART peripheral.
2. Start UART communication.
3. Receive data from the serial terminal.
4. Read the received data.
5. Transmit the received data back to the terminal.
6. Repeat the communication process.

## OBSERVATION

UART reception and echo communication were demonstrated successfully using a serial terminal.

## INFERENCE

The experiment demonstrates UART data reception and echo functionality using the STM32 Blue Pill. It provides practical understanding of bidirectional serial communication using STM32 HAL libraries.