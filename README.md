<p align="center"><img width="256" src="./.assets/logo.png" alt="narvi logo"></p>

Evolved from being just an idea to a completed prototype design. This repository will contain schematics, rendered board views and also firmware sources with USB-HID driver apps to control some of the devices features from the user operating system.



## Introduction

**narvi** (*/ˈnɑːrvi/*) is a device that allows to share some USB enabled devices (like a keyboard, mice, serial port interface, etc.) and an integrated microSD card reader with two host devices within just a tiny little box. Additionally it features a quick charge 3.0 front interface and an LED strip connector (for desk lighting or whatever).

The idea to create such a device came from day to day usage of a Macbook with a desktop PC next to. Manually switching the keyboard or mice connection most of the time is a pain in the ass. This eliminates such annoyances and allows to switch the host connection with just a button press (later on probably with a shortcut in the operating system, without even touching the device). Additionally it features an integrated microSD card reader for the selected host and an USB charger upfront with quick charge 3.0 capable interface without disturbing any of the USB communications.



## Hardware

<p align="center"><img width="512" src="./.assets/pcb_top_assembly.png" alt="pcb top assembly"></p>

The devices hardware consists of the following main components:

- **TPS54229** – Buck Converter ICs that provide both 5V and 3.3V rails for the whole device. The 5V rail supplies all devices that are connected through the USB ports,
- **TS3USB221** – USB Switch ICs providing the host-switch capability,
- **GL850G** – Main USB Hub Controller with supplied EEPROM on-board to customize its properties,
- **USB2241** – MicroSD Card Reader Controller,
- **IP6518** – Front USB Quick Charge 3.0 Compatible Controller,
- **STM32F103T8U6** – Brain of the device, providing an integrated USB controller connected directly to the main hub controller.



## Project state

Waiting for components to arrive from China. Unless Royal Mail decides eventually to deliver my packet, I am stuck at the current draft state. _Meh._



## License

<p align="center"><a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a></p>
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

