<p align="center">
  <img src="assets/banner.svg" width="100%" alt="Arnold Ackom Oduro — Embedded systems, PCB design and C/C++" />
</p>

<p align="center">
  <a href="#featured-projects"><img src="assets/button-projects.svg" alt="Explore my projects" /></a>
  <a href="#build-notes"><img src="assets/button-notes.svg" alt="Read my build notes" /></a>
  <a href="https://www.linkedin.com/in/arnold-ackom-oduro-41820b33b/"><img src="assets/button-linkedin.svg" alt="Connect with Arnold on LinkedIn" /></a>
</p>

I’m building my skills through hands-on electronics and microcontroller projects. I enjoy taking a circuit from schematic to assembled hardware, finding out why it fails, and improving the next version.

## Engineering snapshot

```yaml
hardware: [Schematics, PCB layout, Routing, Assembly]
code:     [C, C++]
approach: "Build → troubleshoot → improve → document"
```

## Tools and interfaces

<p>
  <a href="#engineering-snapshot"><img src="assets/badge-c.svg" alt="C programming" /></a>
  <a href="#engineering-snapshot"><img src="assets/badge-cpp.svg" alt="C++ programming" /></a>
  <a href="#usb-type-c-charger"><img src="assets/badge-kicad.svg" alt="KiCad PCB design" /></a>
  <a href="#stm32f446-development-board"><img src="assets/badge-stm32.svg" alt="STM32 projects" /></a>
  <a href="#home-intrusion-detection-system"><img src="assets/badge-esp32.svg" alt="ESP32 projects" /></a>
</p>

**Communication interfaces of interest:** UART · SPI · I²C · USB · CAN

## Featured projects

### STM32F446 Development Board
**Current project · First prototype preparation**

A custom four-layer development board covering schematic design, component selection, PCB layout, routing and assembly preparation. I’m documenting the design decisions and revisions as the project progresses.

Hardware has not yet been bench-tested. Fabrication stackup confirmation and final assembly review are still pending.

### USB Type-C Charger
**KiCad · PCB etching · Hand assembly**

Designed a USB Type-C charger from scratch in KiCad, completing the schematic, PCB layout and routing with guidance from my mentor and without AI assistance. A subsequent prototype successfully charged a phone after my first board failed.

### Home Intrusion Detection System
**ESP32 · Sensors · GSM alerts**

Built an ESP32-based prototype combining PIR motion detection, magnetic door sensing and vibration sensing. The system included a SIM800L GSM module for SMS alerts, a keypad for password-based arming and disarming, and an I²C LCD with audible and LED status indicators.

## Build notes

<details>
<summary><strong>USB charger: fabrication, assembly and lessons learned</strong></summary>

I etched the PCB using ferric chloride, manually placed and hand-soldered the components, and tested the assembled board.

The first prototype failed, which I attributed to inadequate current protection. I revised the design and got the subsequent prototype to charge a phone. The experience developed my practical skills in PCB fabrication, soldering and hardware troubleshooting.

</details>

<details>
<summary><strong>Intrusion system: key components and their roles</strong></summary>

| Component | Purpose |
|---|---|
| ESP32 | Processes sensor inputs and controls the system |
| HC-SR501 PIR, magnetic reed switch and SW-420 | Motion, door/window opening and vibration detection |
| SIM800L | GSM interface for SMS alerts |
| 4×4 keypad | Password entry for arming and disarming |
| I²C LCD, buzzers and LEDs | System messages, alarms and status feedback |

</details>

---

Project documentation, design iterations and test results will grow with the work. [Connect on LinkedIn](https://www.linkedin.com/in/arnold-ackom-oduro-41820b33b/).
