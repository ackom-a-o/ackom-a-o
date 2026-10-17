# Home Intrusion Detection System

[← Back to my profile](https://github.com/ackom-a-o)

**Arduino Mega · C++ / Arduino framework · Group project**

A home intrusion detection prototype built as a group project for COE 381 (Microprocessors) at KNUST. The system combines proximity and motion sensing with keypad PIN authentication, an LCD and local audible and visual feedback. The physical build used an Arduino Mega; the Tinkercad presentation shows an Uno-based simulation.

## My contribution

I collaborated on building and testing the prototype, and presented the components used and their roles in the system. The firmware and report are credited to the project team, COE 381 Group 4.

## Hardware and operation

| Component | Role |
|---|---|
| Arduino Mega 2560 | Reads inputs and controls system behaviour |
| HC-SR04 ultrasonic sensor | Detects nearby objects |
| PIR motion sensor | Detects movement |
| 4×4 matrix keypad | Accepts PIN input |
| 16×2 I²C LCD | Displays prompts and system status |
| RGB LED and two buzzers | Provide visual status and local alarm feedback |

The documented behaviour covers idle, PIN entry, access granted, alert and alarm conditions. The presentation video shows the assembled model-house prototype, keypad interaction, an illuminated LCD and changing status lights. These observations do not independently verify every reported test case.

## Firmware and original group material

- [Original group repository](https://github.com/enkadi/Home-Intrusion-System)
- [Standalone C++ source](https://github.com/enkadi/Home-Intrusion-System/blob/b7dec187a0fdef24d7db9c69b55d3e5197c770e9/security_system.cpp)
- [Group report, including the Mega pin assignments and firmware listing](https://github.com/enkadi/Home-Intrusion-System/blob/b7dec187a0fdef24d7db9c69b55d3e5197c770e9/COE381%20Group4%20HomeIntrusionSystem.pdf)

The standalone source and report contain different firmware versions:

| Detail | Standalone source | Report listing |
|---|---|---|
| LCD | No LCD code | I²C LCD support |
| PIR input | Pin 2 | Pin 43 |
| Keypad columns | Pins 9–12 | Pins 22–25 |
| Timing | Uses blocking delays | Uses `millis()` for alarm effects, with blocking operations elsewhere |

The versions must be reconciled against the physical wiring before reuse. Neither has been newly compiled or hardware-tested as part of this portfolio review. No reuse licence was found in the inspected repository, so the original code and report are linked here rather than copied.

## Scope and next step

This was an educational prototype with local feedback. Remote notifications remain a possible future extension.

The next technical step is to confirm the final wiring and firmware version, then document repeatable tests for PIN handling, sensor triggers, alarm activation and reset.
