# Home Intrusion Detection System

[← Back to my profile](https://github.com/ackom-a-o)

**ESP32 · Sensors · GSM alerts**

Built an ESP32-based prototype combining PIR motion detection, magnetic door sensing and vibration sensing. The system included a SIM800L GSM module for SMS alerts, a keypad for password-based arming and disarming, and an I²C LCD with audible and LED status indicators.

## Main components

| Component | Purpose |
|---|---|
| ESP32 | Processes sensor inputs and controls the system |
| HC-SR501 PIR, magnetic reed switch and SW-420 | Motion, door/window opening and vibration detection |
| SIM800L | GSM interface for SMS alerts |
| 4×4 keypad | Password entry for arming and disarming |
| I²C LCD, buzzers and LEDs | System messages, alarms and status feedback |

## Evidence status

This is a summary of the ESP32 prototype I built. Schematics, firmware, photos and function-by-function test results are not yet included here.
