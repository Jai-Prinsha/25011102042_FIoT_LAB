# CAT 12 (C) – Short-Press and Long-Press Detection

## EXPERIMENT

CAT 12

## DATE

[Enter Experiment Date]

## NAME OF EXPERIMENT

Short-Press and Long-Press Detection

## HARDWARE SETUP / PLATFORM

- NUCLEO-F410RB
- On-board LED (LD2 – PA5)
- User Button (B1 – PC13)
- STM32CubeMX
- Keil MDK-ARM
- STM32 HAL Library

## AIM

To differentiate short and long button presses and control LED operations using non-blocking timing.

## IMPLEMENTATION

1. Implement button debouncing.
2. Use a 1-second threshold to distinguish short and long presses.
3. Use a short press to toggle the LED.
4. Use a long press to activate continuous LED blinking.
5. Use HAL_GetTick() for non-blocking timing.

## WORKING PRINCIPLE

- The button state is monitored using PC13.
- Debouncing is implemented to avoid multiple detections.
- HAL_GetTick() records and measures the button press duration.
- A press shorter than 1 second is treated as a short press and toggles the LED.
- A press lasting 1 second or more is treated as a long press and activates continuous LED blinking.
- Non-blocking timing allows the program to continue executing without waiting in a blocking delay.

## CIRCUIT DIAGRAM

![LED and User Button Circuit](circuit.png)

## CORE LOGIC / PSEUDOCODE

1. Initialize GPIO peripherals.
2. Configure PA5 as output and PC13 as input.
3. Detect a button press.
4. Record the press start time using HAL_GetTick().
5. Measure the press duration.
6. If the duration is less than 1 second, toggle the LED.
7. If the duration is 1 second or more, activate continuous LED blinking.
8. Repeat the process.

## OBSERVATION

The LED responded differently to short and long button presses.

## INFERENCE

The experiment demonstrates button debouncing, press-duration measurement, and LED control using non-blocking timing with HAL_GetTick() on the NUCLEO-F410RB development board.