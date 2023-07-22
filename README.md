# Project-2537_5b7a_0023-Led-driver

This repository contains the KiCad circuit design for this project.

## Components

- Microcontroller: Microchip PIC18F97J60
- PoE Controller: Onsemi NCP1095DBR2
- Constant Current Drivers: TI LM3405A
- LEDs: Lumiled Rebels (x5)

## Description

The circuit design aims to control the brightness of five Lumiled Rebels LEDs individually via Ethernet data transfer using the STM32 microcontroller. The entire circuit is powered through PoE (Power over Ethernet) using the Onsemi PoE controller.

## Directory Structure

- `Schematics/`: KiCad schematic files (.sch) for the main circuit.
- `PCBLayout/`: KiCad PCB layout files (.kicad_pcb) for the circuit.
- `Documentation/`: Any relevant documentation or datasheets used in the design.
