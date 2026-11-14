# CAT 10(C) – ESP8266 Wi-Fi Connection

## EXPERIMENT

Continuous Lab Evaluation – 10

## DATE

[Enter Experiment Date]

## NAME OF EXPERIMENT

Wi-Fi Connection Using ESP8266

## HARDWARE SETUP / PLATFORM

- STM32 Blue Pill (STM32F103C8T6)
- ESP8266 / Wemos Wi-Fi Module
- USB-to-TTL Converter
- STM32CubeMX
- Keil MDK-ARM
- STM32 HAL Library

## AIM

To connect the ESP8266 module to a Wi-Fi network using AT commands and verify the network connection response.

## IMPLEMENTATION

1. Configure the ESP8266 Wi-Fi mode.
2. Send AT commands to connect to a Wi-Fi network.
3. Receive and check the connection response.
4. Verify successful network connectivity.

## WORKING PRINCIPLE

- STM32 communicates with ESP8266 through UART.
- The required Wi-Fi operating mode is configured.
- Wi-Fi connection commands are sent to the module.
- ESP8266 attempts to connect to the specified network.
- The returned response is checked to verify connectivity.

## CIRCUIT DIAGRAM



## CORE LOGIC / PSEUDOCODE

1. Initialize GPIO and UART peripherals.
2. Establish UART communication with ESP8266.
3. Send the required AT command.
4. Receive and verify the response.
5. Configure the Wi-Fi operating mode.
6. Send the Wi-Fi connection command.
7. Receive the connection response.
8. Verify successful network connectivity.

## INFERENCE

The experiment demonstrates how to configure the ESP8266 Wi-Fi mode and connect to a wireless network using AT commands. It provides practical understanding of UART-based Wi-Fi module control and network connectivity.
