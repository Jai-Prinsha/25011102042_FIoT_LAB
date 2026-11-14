# CAT 10 (B) – ESP8266 AT Commands

## EXPERIMENT

Continuous Lab Evaluation – 10

## DATE

[Enter Experiment Date]

## NAME OF EXPERIMENT

ESP8266 AT Command Testing

## HARDWARE SETUP / PLATFORM

- STM32 Blue Pill (STM32F103C8T6)
- ESP8266 / Wemos Wi-Fi Module
- USB-to-TTL Converter
- STM32CubeMX
- Keil MDK-ARM
- Arduino IDE (for module testing)
- STM32 HAL Library

## AIM

To explore and test the AT command interface of the ESP8266 module and examine its firmware and Wi-Fi configuration responses.

## IMPLEMENTATION

1. Test basic AT commands.
2. Check module firmware information.
3. Explore Wi-Fi configuration commands.
4. Test network-related commands and examine module responses.

## WORKING PRINCIPLE

- AT commands are sent to the ESP8266 through a serial interface.
- The module processes each command.
- The ESP8266 returns responses indicating the command status.
- Firmware information and Wi-Fi-related settings are examined.

## CIRCUIT DIAGRAM



## CORE LOGIC / PSEUDOCODE

1. Initialize UART communication.
2. Send basic AT commands.
3. Receive and verify module responses.
4. Check firmware information.
5. Explore Wi-Fi configuration commands.
6. Test network-related commands.
7. Examine the received responses.

## INFERENCE

The experiment demonstrates the use of ESP8266 AT commands to examine module firmware, Wi-Fi configuration, and network-related functions.
