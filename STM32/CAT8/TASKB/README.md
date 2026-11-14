# CAT8 – STM32 GPIO Bring-Up and Switch-Controlled LED

## EXP
Continuous Lab Evaluation – 8 (TASK B)

## DATE
18/09/2026 (Week 8)

## NAME OF EXP
Event-Based LED Control with Software Debouncing

## HARDWARE SETUP / PLATFORM
- **Microcontroller:** STM32 Blue Pill
- **Development Tool:** STM32CubeMX
- **IDE / Compiler:** Keil MDK
- **Programming Language:** Embedded C
- **Libraries:** STM32 HAL Libraries
- **Hardware:** Push-Button, LED, Current-Limiting Resistor, Breadboard and Jumper Wires

## TASK NO

### Task 8B – Event-Based Control

**Problem Statement:**

Modify the firmware so each valid switch press toggles the LED state. Investigate switch bounce and implement software debouncing so one press produces one toggle.

**Core Logic:**
1. Read the push-button state.
2. Detect a valid button press.
3. Apply software debouncing.
4. Toggle the LED only once for each valid press.
5. Wait for the button release before detecting the next press.

## CIRCUIT DIAGRAM

The same push-button and LED circuit is used for Tasks 8A, 8B and 8C.

![TASK B Circuit Diagram](circuit.png)

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

### General Pseudocode
1. Start.
2. Initialize GPIO pins.
3. Configure the button as input and LED as output.
4. Read the push-button state.
5. Detect a valid button press.
6. Apply software debouncing.
7. Toggle the LED once for each valid press.
8. Wait for the button release.
9. Repeat continuously.

### Code Base
- `cat8_taskB_debounce.c`
- STM32CubeMX project file (`.ioc`)
- Keil project file (`.uvprojx`)
- Generated HAL files, if required

## INFERENCE

The experiment demonstrates event-based LED control using STM32 GPIO. Software debouncing is implemented to avoid multiple LED toggles caused by switch bounce, ensuring one toggle for each valid button press.