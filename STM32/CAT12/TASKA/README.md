# CAT 12 (A) – On-board LED Bring-Up

## EXPERIMENT

CAT 12

## DATE

[Enter Experiment Date]

## NAME OF EXPERIMENT

On-board LED Bring-Up

## HARDWARE SETUP / PLATFORM

- NUCLEO-F410RB
- STM32CubeMX
- Keil MDK-ARM
- STM32 HAL Library

## AIM

To configure and control the on-board LED of the NUCLEO-F410RB development board using GPIO operations.

## IMPLEMENTATION

1. Configure PA5 as GPIO output.
2. Initialize the GPIO peripheral.
3. Implement LED blinking using GPIO operations.

## WORKING PRINCIPLE

- PA5 is configured as a GPIO output pin.
- The GPIO peripheral is initialized.
- The LED connected to PA5 is controlled using GPIO operations.
- The LED is repeatedly turned ON and OFF to produce blinking.

## CIRCUIT DIAGRAM

![On-board LED Circuit](circuit.png)

## CORE LOGIC / PSEUDOCODE

1. Initialize GPIO peripherals.
2. Configure PA5 as output.
3. Set the LED pin HIGH.
4. Provide a delay.
5. Set the LED pin LOW.
6. Provide a delay.
7. Repeat the process.

## OBSERVATION

The on-board LED blinked as expected.

## INFERENCE

The experiment demonstrates GPIO output configuration and on-board LED control using the NUCLEO-F410RB development board.