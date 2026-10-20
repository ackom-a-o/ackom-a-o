# STM32F446 Development Board

[← Back to my profile](https://github.com/ackom-a-o)

**🛠️ Custom hardware · Arm Cortex-M4 · Four-layer PCB**

I’m designing a USB-powered development board around the **STM32F446ZET6**, taking it from schematics and component selection through PCB layout, assembly preparation and prototype bring-up. It is a platform for learning embedded systems and experimenting with sensors, communications and control.

### 🔎 Explore the public project

**[Open the design repository →](https://github.com/ackom-a-o/stm32f446-development-board)**

[📄 Schematic PDF](https://github.com/ackom-a-o/stm32f446-development-board/blob/main/docs/schematic.pdf) · [🧩 Design decisions](https://github.com/ackom-a-o/stm32f446-development-board/blob/main/docs/design-decisions.md) · [✅ Validation evidence](https://github.com/ackom-a-o/stm32f446-development-board/blob/main/docs/validation.md)

## The board

[![STM32F446 PCB top copper and silkscreen](https://raw.githubusercontent.com/ackom-a-o/stm32f446-development-board/main/docs/images/pcb-top.png)](https://github.com/ackom-a-o/stm32f446-development-board)

*KiCad design view showing top copper and silkscreen; the first assembled prototype is still ahead.*

| Feature | Implementation |
|---|---|
| Processor | STM32F446ZET6 · Arm Cortex-M4 · LQFP-144 |
| Board | 80 × 70 mm · four copper layers · nominal 1.6 mm |
| Power | USB 5 V → protection → 3.3 V regulator → load switch |
| Interfaces | USB full-speed device, SPI, I²C, UART, analogue inputs and GPIO |
| CAN expansion | CAN1 on PD0/PD1 through J7; external transceiver required |
| Programming | External SWD probe through a custom five-pin header |
| Clock and controls | 8 MHz crystal, three pushbuttons and three indicator LEDs |

## 🧠 What I’m working through

- **Power design:** protection, regulator headroom, decoupling and startup behaviour.
- **PCB layout:** component placement, ground returns, USB routing and thermal paths.
- **Readable schematics:** four functional sheets, with MCU power and ports separated for review.
- **Assembly preparation:** exact part matching, custom footprints, connector placement and component orientation.
- **Verification:** electrical and PCB rule checks, schematic-to-layout consistency, datasheet review and a staged test plan.

One example of the iteration: repositioning the reset capacitor shortened its routed connection from **19.45 mm to 13.41 mm**. The repository records both the improvement and the remaining layout compromises.

## 🚧 Current milestone

**First prototype preparation — final design and assembly review.** The fabricator has confirmed the intended stackup. A further pre-order review identified local bypassing and ground-return improvements to address before release.

Hardware has **not yet been bench-tested**. Next comes controlled first power-up, rail measurements, SWD/reset checks, clock validation and USB communication testing. Firmware and measured results will be added as that work progresses.

[Follow the validation record and test plan →](https://github.com/ackom-a-o/stm32f446-development-board/blob/main/docs/validation.md)

## 📂 Want to inspect the actual design?

The public repository contains the **editable KiCad schematics and routed PCB**, project libraries, schematic PDF, part inventory and engineering notes. Open **stm32.kicad_pro** in **KiCad 10** to explore the hardware.

**[View all project files →](https://github.com/ackom-a-o/stm32f446-development-board)**
