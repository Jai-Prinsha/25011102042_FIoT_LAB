# CAT 2 – 8051 Bare-Metal LED Blinking

**Course:** 25CS2741 – Fundamentals of Internet of Things + Lab  
**Experiment:** Continuous Lab Evaluation – 2  
**Date:** 20/07/2026 (Week 2)  
**Platform:** 8051 Development Board – AT89S52

## Aim
To compile a minimal bare-metal C program, program the AT89S52 microcontroller, and blink an LED by directly accessing GPIO registers.

## Hardware Requirements
- AT89S52 Microcontroller
- 8051 Development Board
- LED
- Programmer / Debugger
- Power Supply
- Connecting Wires

## Software Requirements
- Keil µVision
- Embedded C
- 8051 Device Support

## Hardware Bring-Up
| Parameter | Student Entry |
|---|---|
| MCU | AT89S52 |
| CPU Core | 8051 |
| Operating Voltage | 5V (verify board supply) |
| Debug Interface | Board programmer |
| LED GPIO Port | Port 1 |
| LED GPIO Pin | P1.0 (assumed; verify schematic) |
| LED Active State | Active HIGH (assumed) |
| LED Frequency | Approximately 1 Hz |

## Procedure
1. Identify the AT89S52 microcontroller and development board.
2. Verify the board power supply.
3. Identify the LED GPIO pin from the board schematic.
4. Create a C program using Keil µVision.
5. Configure the LED pin using direct register access.
6. Implement a software delay function.
7. Compile and generate the HEX file.
8. Program the microcontroller and observe LED blinking.

## Code
See `main.c`.

## Custom Delay Function
The `delay_ms()` function generates an approximate software delay using nested loops.

## Inference
The AT89S52 microcontroller was programmed using bare-metal Embedded C. The LED was controlled through direct GPIO register access, and a custom software delay function was implemented to produce approximately 1 Hz blinking.

## Result
The bare-metal LED blinking program was compiled and tested on the AT89S52 development board.
