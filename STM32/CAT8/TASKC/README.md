# CAT8 – STM32 GPIO Bring-Up and Switch-Controlled LED

## EXP
Continuous Lab Evaluation – 8 (TASK C)

## DATE
18/09/2026 (Week 8)

## NAME OF EXP
Short Press and Long Press Detection Using STM32

## HARDWARE SETUP / PLATFORM
- **Microcontroller:** STM32 Blue Pill
- **Development Tool:** STM32CubeMX
- **IDE / Compiler:** Keil MDK
- **Programming Language:** Embedded C
- **Libraries:** STM32 HAL Libraries
- **Hardware:** Push-Button, LED, Current-Limiting Resistor, Breadboard and Jumper Wires

## TASK NO

### Task 8C – Short Press vs Long Press

**Problem Statement:**

Classify button presses based on duration and perform different LED operations.

**Press Duration:**
- **Short press:** Less than 1 second.
- **Long press:** 1 second or more.

**Expected Behaviour:**

| User Action | System Response |
|---|---|
| Short press | Toggle LED |
| Long press | LED enters continuous blinking mode |
| Next short press | Stop blinking |
| Long press again | Return to blinking mode |

**Important Constraint:**

Do not use a blocking delay to determine whether a button is held for a long press. Use a non-blocking time measurement approach.

**Core Logic:**
1. Detect the button press and record the start time using `HAL_GetTick()`.
2. Continuously monitor the button state.
3. Calculate the press duration without blocking the program.
4. If the duration is less than 1 second, toggle the LED.
5. If the duration is 1 second or more, activate or deactivate blinking mode.
6. Continue monitoring button events.

## CIRCUIT DIAGRAM

The same push-button and LED circuit is used for Tasks 8A, 8B and 8C.

![TASK C Circuit Diagram](circuit.png)

**Hardware Components:**
- STM32 Blue Pill development board
- Push-button
- LED
- Current-limiting resistor
- Breadboard and jumper wires

*Note: Add the actual hardware circuit diagram as `circuit.png`. Pin connections must match the source code.*

## CORE LOGIC / PSEUDOCODE / CODE BASE

### Core HAL Functions
- `HAL_GPIO_ReadPin()` – Read switch state.
- `HAL_GPIO_WritePin()` – Control LED.
- `HAL_GPIO_TogglePin()` – Toggle LED.
- `HAL_GetTick()` – Measure button press duration.
- `HAL_Delay()` – Optional delay; not used for measuring long-press duration.

### General Pseudocode
1. Start.
2. Initialize GPIO pins.
3. Record the button press start time using `HAL_GetTick()`.
4. Continuously monitor the button state.
5. Calculate the press duration.
6. If duration is less than 1 second, toggle the LED.
7. If duration is 1 second or more, activate or deactivate blinking mode.
8. Continue monitoring button events.

### Code Base
- `cat8_taskC_short_long_press.c`
- STM32CubeMX project file (`.ioc`)
- Keil project file (`.uvprojx`)
- Generated HAL files, if required

## INFERENCE

The experiment demonstrates short-press and long-press detection using STM32 GPIO and HAL functions. The `HAL_GetTick()` function is used for non-blocking time measurement, allowing different LED operations based on button press duration.