# CAT 12 (B) – On-board Switch Control with State Remembrance

## EXPERIMENT

CAT 12

## DATE

[Enter Experiment Date]

## NAME OF EXPERIMENT

On-board Switch Control with State Remembrance

## HARDWARE SETUP / PLATFORM

- NUCLEO-F410RB
- On-board LED (LD2 – PA5)
- User Button (B1 – PC13)
- STM32CubeMX
- Keil MDK-ARM
- STM32 HAL Library

## AIM

To control the on-board LED using the user button and maintain its previous state until the next valid button press.

## IMPLEMENTATION

1. Configure PC13 as GPIO input.
2. Configure PA5 as GPIO output.
3. Detect valid button presses.
4. Toggle the LED state whenever a valid button press is detected.
5. Maintain the LED's state until the next valid press.

## WORKING PRINCIPLE

- PC13 is configured as a GPIO input to detect button presses.
- PA5 is configured as a GPIO output to control the LED.
- A valid button press is detected.
- The LED state is toggled.
- The updated state is maintained until another valid press occurs.

## CIRCUIT DIAGRAM

![LED and User Button Circuit](circuit.png)

## CORE LOGIC / PSEUDOCODE

1. Initialize GPIO peripherals.
2. Configure PC13 as input.
3. Configure PA5 as output.
4. Read the button state.
5. Detect a valid button press.
6. Toggle the LED state.
7. Maintain the current LED state.
8. Repeat the process.

## OBSERVATION

Each valid button press changed the LED state.

## INFERENCE

The experiment demonstrates GPIO input and output operations using the on-board button and LED. It also explains how to maintain LED state using software logic.