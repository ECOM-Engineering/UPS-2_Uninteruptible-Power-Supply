# UPS-2 Uninterruptible Power Supply 

## Hat Solution For Raspberry pi Computers

- Compatible with Raspberry models 3, 3B, 4B
- High efficiency power supply with output 5V, 3A
- Main input voltage range 6.5V ... 20V
- Efficiency > 95% at main input 12V
- Battery standby current < 8uA @9V
- Battery voltage 6V ... 20V
- Nearly no self heating
- Communication with Pi via serial UART or parallel port
- Python library for unattended operation and optional GUI

## Project Components

- UPS-2  Hardware Hat module 
- UPS-2 hat firmware for power supply written in C
- Raspberry pi  software for pi written in Python3

### UPS-2 Hat Module

**Details in repository UPS-2**_Hardware

![UPS-2_cut](F:\kDrive\Projekte\Raspberry\UPS-2\UPS-2-Project-repository\UPS-2_Uninteruptible-Power-Supply\images\UPS-2_cut.png)



### UPS-2 Hat Firmware

Firmware is running on the hat's STM32-G030 CPU for serial or parallel communication with the Raspberry  computer.

**Details in repository** [UPS-2_PowerSupply_SW](https://github.com/ECOM-Klaus/UPS-2_PowerSupply_SW.git)

### UPS-2 Raspberry Software

Python scripts for communication with the UPS-2 hat and optionally with user software.

**Details in repository** [UPS-2_Raspberry_SW](https://github.com/ECOM-Klaus/UPS-2_Raspberry_SW.git)

