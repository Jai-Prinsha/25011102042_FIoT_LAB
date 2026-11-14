# CAT 10 (A)– UART Communication with ESP8266

## EXPERIMENT

Continuous Lab Evaluation – 10 Task A


## NAME OF EXPERIMENT

UART Communication with ESP8266

## HARDWARE SETUP / PLATFORM

- STM32 Blue Pill (STM32F103C8T6)
- ESP8266 / Wemos Wi-Fi Module
- USB-to-TTL Converter
- STM32CubeMX
- Keil MDK-ARM
- STM32 HAL Library

## AIM

To establish UART communication between STM32 Blue Pill and ESP8266 and exchange AT commands and responses.

## IMPLEMENTATION

1. Configure UART communication using STM32CubeMX.
2. Initialize UART using STM32 HAL functions.
3. Send AT commands from STM32 to ESP8266.
4. Receive and examine responses from the ESP8266 module.

## WORKING PRINCIPLE

- UART provides serial communication between STM32 and ESP8266.
- STM32 sends AT commands through UART.
- ESP8266 processes the received commands.
- The module sends responses back to STM32.

## CIRCUIT DIAGRAM



## CORE LOGIC / PSEUDOCODE

1. Initialize GPIO and UART peripherals.
2. Establish UART communication with ESP8266.
3. Send the AT command.
4. Receive the response from ESP8266.
5. Examine the received response.
6. Repeat the communication process.

## INFERENCE

The experiment demonstrates UART communication between STM32 and ESP8266. It provides practical understanding of serial data transmission, AT command communication, and response reception.
