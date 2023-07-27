# LED Driver Circuit

Welcome to my photogrammetry project! Within this repository, you will find the KiCad PCB design, as well as the firmware for the LED driver circuit. The LED driver circuit is a crucial component in my photogrammetry project.

## Introduction

My photogrammetry project focuses on creating photorealistic digital clones using a low-budget image capture system with precise illumination facilitated by several LED driver circuits. Precise, multispectral lighting is important for accurate image capture. The images captured are used to recreate texture maps, including diffuse, specular, and roughness maps. Additionally, the images captured serve as valuable training data for creating deepfake models.

The LED driver circuit consists of constant current drivers powering five LEDs, including RGB LEDs, a PC Amber LED, and a neutral white LED. Each circuit incorporates a cost-effective 8-bit Microchip PIC16 microcontroller. Ethernet communication between a main computer through a Power over Ethernet (PoE) switch will be used<sup><a href="#item1">[1]</a></sup>. The microcontroller will most likely implement a lightweight TCP/IP stack where a main computer sends either UDP or TCP packets. While a UDP or TCP packet can be sent via simple commands from the main computer, a custom application will be developed to automate this process once several LED driver circuits are implemented.

Please note that the resources herein are intended solely for this specific project and should not be used elsewhere. My intent for creating the photogrammetry project is my own personal use, and is not intended to create digital clones of anyone besides myself.

## Components

Some important components included in the schematic:

- Microchip PIC16F18026
- Microchip PD70210
- Cree LED JE2835 3V N-Class LEDs
- Luxeon 2835E Neutral White LEDs

## Directory Structure

- `LED-driver-kicad/`: KiCad schematic files (.sch), KiCad PCB layout files (.kicad_pcb) for the main circuit.
- `firmware/`: Any firmware-related code for the microcontroller.
- `Documentation/`: Any relevant documentation or datasheets used in the design.

## References

<ol>
<li id="item1">
“IEEE Standard for Information technology-- Local and metropolitan area networks-- Specific requirements-- Part 3: CSMA/CD Access Method and Physical Layer Specifications Amendment 3: Data Terminal Equipment (DTE) Power via the Media Dependent Interface (MDI) Enhancements” <i>IEEE Standards Association</i>, 30 Oct. 2009, <a href="https://standards.ieee.org/ieee/802.3at/4553/" target="_blank" rel="noopener noreferrer">standards.ieee.org/ieee/802.3at/4553/</a>.
</li>
</ol>
