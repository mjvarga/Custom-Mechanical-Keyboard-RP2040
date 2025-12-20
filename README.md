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
