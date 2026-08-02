# USB-C Breadboard Power Supply

A compact USB-C Power Delivery (PD) breadboard power supply designed for electronics prototyping and development.
The board is based on the **CH224K USB-PD sink/trigger IC** and is designed to obtain power from compatible USB-C PD adapters and provide it conveniently to standard breadboard power rails.
## PCB 3D View
<h2>PCB 3D View</h2>

<p align="center">
  <img src="Images/PCB_3D_F.png" width="700">
</p>
<h2>PCB 3D View</h2>

<p align="center">
  <img src="Images/PCB_3D_B.png" width="700">
</p>

## Features

- USB Type-C power input
- CH224K USB-PD sink/trigger controller
- Selectable USB-PD voltage configuration
- 3-position DIP switch
- Breadboard-compatible 2.54 mm headers
- Power indicator LED
- 100 µF input/output filtering capacitors
- Compact PCB design
- Custom AT PCB logo
- KiCad schematic and PCB source files included

---

## Hardware

### Main Components

| Component | Description |
|---|---|
| CH224K | USB Power Delivery sink/trigger controller |
| USB-C Receptacle | USB-C power input |
| DIP Switch | PD voltage configuration |
| LED | Power indication |
| 100 µF / 35 V | Power filtering capacitors |
| 2.54 mm Headers | Breadboard power connections |

---

## USB-C Power Delivery

The CH224K communicates with a compatible USB-C PD power adapter and requests an appropriate power profile according to the hardware configuration.

> **Important:** Available output voltages and current depend on the USB-C PD adapter being used and the CH224K configuration.

A charger rated for 33 W does not continuously deliver 33 W to the board. The connected load draws the current it requires, up to the limits of the negotiated USB-PD profile and the hardware.

---

## Breadboard Interface

The PCB is designed to plug directly into the positive and negative power rails of a standard solderless breadboard using **2.54 mm male headers**.

This makes it useful for quickly powering:

- Microcontroller projects
- Sensors
- Development boards
- Analog circuits
- Digital circuits
- General breadboard prototypes

---

## Project Structure

```text
USB-C-Breadboard-Power-Supply/
│
├── USB-C Breadboard Power Supply.kicad_pro
├── USB-C Breadboard Power Supply.kicad_sch
├── USB-C Breadboard Power Supply.kicad_pcb
│
├── My_Logos.pretty/
│   └── AT_Logo.kicad_mod
│
├── Gerber/
│   └── Manufacturing files
│
├── Images/
│   └── PCB and schematic images
│
└── README.md
