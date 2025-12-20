# Custom-Mechanical-Keyboard-RP2040

This project documents the design and implementation of a custom mechanical keyboard built around the Raspberry Pi RP2040 microcontroller, covering the full workflow from schematic capture and multilayer PCB design to firmware configuration, assembly, and validation.

The keyboard was designed as a USB HID device and includes regulated 3.3 V power delivery, matrix-scanned keys, custom programmable lighting, and support for fully configurable keymaps and macros using QMK/VIA firmware. The PCB was designed with power-integrity and EMI-aware layout practices, including proper decoupling, grounding strategy, and manufacturability checks.

The completed keyboard is fully functional and used for personal use, primarily for custom shortcut entry in CAD workflows, providing real-world validation of reliability and performance.

This project was inspired by and based on open-source reference designs by Robert Feranec, adapted and extended to gain hands-on experience with embedded systems design, PCB layout, and hardware–firmware co-design.

# Features

* RP2040-based USB HID mechanical keyboard

* Multilayer PCB with dedicated power and ground planes

* Matrix-scanned keys with configurable layouts

* Programmable lighting with firmware-controlled effects

* QMK/VIA support for dynamic keymaps and macros

Designed for long-term daily use and reliability

# Hardware Overview

* Microcontroller: Raspberry Pi RP2040

* Power: USB-powered with on-board 3.3 V regulation and decoupling network

* PCB: Multilayer design with EMI-aware routing and grounding strategy

* Input: Mechanical key switches arranged in a scanned matrix

* Lighting: Addressable LEDs integrated into the PCB and controlled via firmware

* Debugging: SWD interface for programming and debugging

# Firmware

* Fully programmable keymaps and layers

* Custom macros and shortcuts

* Lighting configuration and control

* VIA compatibility for real-time key remapping

<img width="1070" height="758" alt="image" src="https://github.com/user-attachments/assets/fc13ab81-6169-44d6-bf13-efc887fa7a28" />
<img width="1071" height="755" alt="image" src="https://github.com/user-attachments/assets/18153fd4-c7f9-42df-9760-77cd7755fedc" />


# What?
The goal of this project was to design and build a fully functional custom mechanical keyboard based on the Raspberry Pi RP2040, serving both as a programmable macro tool to improve workflow efficiency and as a platform to gain hands-on experience with multilayer PCB design, embedded hardware–firmware co-design, and USB HID devices.

# How?
* Designed the keyboard schematic and multilayer PCB in EasyEDA, including USB power input, 3.3 V regulation, and matrix-scanned key inputs
* Integrated the RP2040 microcontroller, external flash, SWD debug interface, and supporting passive components following reference designs
* Applied power integrity and EMI-aware layout techniques, including decoupling capacitors, grounding strategy, and via stitching
* Implemented custom programmable lighting using addressable LEDs, accounting for signal timing and power budgeting
* Configured and customized QMK/VIA firmware to support programmable keymaps, macros, and lighting control
* Assembled, programmed, and tested the keyboard to verify USB enumeration, stable power delivery, and reliable key detection
  
# Results
* Produced a fully functional custom keyboard that is used daily for CAD shortcut entry and workflow automation
* Strengthened understanding of multilayer PCB layout, grounding, and power distribution in embedded systems
* Gained practical experience reading component datasheets and applying reference designs to real hardware
* Developed confidence in hardware validation through real-world use, beyond simulation or bench testing

# Important References & Resources

The following resources were used during the design, implementation, and validation of this project:

* PCB Impedance Calculator (JLCPCB)
Used to estimate controlled impedance and trace geometry for USB and other high-speed signals during PCB layout.
https://jlcpcb.com/pcb-impedance-calculator

* Cherry MX Switch Datasheet
Reference for switch electrical characteristics, pinout, and mechanical dimensions.
https://cdn.sparkfun.com/datasheets/Components/Switches/MX%20Series.pdf

* WS2812 Addressable LED Datasheet
Used for implementing custom programmable keyboard lighting and estimating power requirements.
https://cdn-shop.adafruit.com/datasheets/WS2812.pdf

* LM3940 Low-Dropout Regulator Datasheet (Texas Instruments)
Reference for 3.3 V power regulation design, dropout characteristics, stability requirements, and decoupling guidelines.
https://www.ti.com/cn/lit/ds/symlink/lm3940.pdf

* Raspberry Pi Pico / RP2040 Datasheet
Primary reference for RP2040 pinout, peripherals, electrical characteristics, and boot configuration.
https://pip-assets.raspberrypi.com/categories/610-raspberry-pi-pico/documents/RP-008307-DS-1-pico-datasheet.pdf

* Würth Elektronik Standoffs (Farnell)
Mechanical reference for PCB mounting and enclosure integration.
https://fr.farnell.com/en-FR/wurth-elektronik/9774035151r/standoff-steel-hex-f-f-m2-5-3/dp/3757968

* QMK Firmware Documentation
Primary reference for firmware configuration, keymaps, macros, and lighting control.
https://qmk.fm/
