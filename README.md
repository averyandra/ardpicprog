# Arduino-based PIC Programmer

![Arduino](https://img.shields.io/badge/-Arduino-00979D?style=for-the-badge&logo=Arduino&logoColor=white)
![C++](https://img.shields.io/badge/-C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/-C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![Microchip](https://img.shields.io/badge/-Microchip-D92A27?style=for-the-badge&logo=microchip&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

---

## About This Fork

This repository is a fork maintained for custom hardware engineering requirements at my **Lab**. 

**Key Modifications:**
* **Added support for PIC16F636:** Extended the original device definitions and programming logic to allow In-Circuit Serial Programming (ICSP) for the PIC16F636 microcontroller using an Arduino Uno.

---

## Project Description

This distribution contains an Arduino-based solution for programming PIC microcontrollers from Microchip Technology Inc, such as the PIC16F628A and friends. The solution has three main parts:

* **Circuit (Hardware):** Built on one or more prototyping shields to interface with the PIC and provide the 13V programming voltage (VPP).
* **Sketch (Firmware):** A sketch called `ProgramPIC` that is loaded into an Arduino to directly interface with the PIC during programming. The sketch implements a simple serial protocol for interfacing with the host.
* **Host Program (Software):** A terminal program called `ardpicprog`; a drop-in replacement for [picprog](http://hyvatti.iki.fi/~jaakko/pic/picprog.html) that implements the serial protocol and controls the PIC programming process from the computer side.

See the [official documentation](http://rweather.github.io/ardpicprog/) for more information on the base project.

## Obtaining ardpicprog

The source code is available in this repository. After cloning, please read the [installation instructions](http://rweather.github.io/ardpicprog/installation.html) for compilation and setup details.

---

## Credits & Original Creator

This project was originally created and developed by **Rhys Weatherley**.

For more information on the original Ardpicprog, to report bugs in the upstream repository, or to suggest improvements, please contact the author via [email](mailto:rhys.weatherley@gmail.com). Patches to support new device types are always welcome.
