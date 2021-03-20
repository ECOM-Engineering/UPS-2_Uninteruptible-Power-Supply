# UPS-2 Uninterruptible Power Supply 

## Hat Solution For Raspberry Pi Computers

UPS-2 is a wide input range, high efficiency power supply for Raspberry Pi computers. It features a main input and a backup input. In case of power fail or under voltage at the main input,  backup input becomes active  with no interruption or spike on the Raspberry 5V, 3A supply output.   
Firmware provides optical and software state feedback, including voltage levels, warnings and CPU temperature.  
UPS-2 can be controlled by software commands from the Raspberry and/or by the on board  push button. Supply commands include POWER OFF, STANDBY and RESTART. 

- Compatible with Raspberry models 3, 3B, 4B
- High efficiency power supply with output 5V, 3A
- Main input voltage range 6.5V ... 20V
- Efficiency > 95% at main input 12V
- Battery standby current < 8uA @9V
- Battery voltage 6.5V ... 20V
- Nearly no self heating thanks to outstanding conversion efficiency
- Communication with Pi via serial UART or parallel port
- Python library for unattended operation and optional GUI



## Project Components

- UPS-2  Hat module hardware
- UPS-2 hat firmware for power supply written in ANSI C
- Raspberry Pi  software written in Python3

### UPS-2 Hat Module Hardware

**Details in repository** [UPS-2_PowerSupply_HW](https://github.com/ECOM-Klaus/UPS-2_PowerSupply_HW)  



![UPS-2_cut](Images/Connections.png) 



### UPS-2 Hat Firmware

Firmware is running on the hat's STM32G030 CPU for serial or parallel communication with the Raspberry  computer.  
**Find details in repository** [UPS-2_PowerSupply_FW](https://github.com/ECOM-Klaus/UPS-2_PowerSupply_FW.git)

### UPS-2 Raspberry Software

Python scripts for communication with the UPS-2 hat and optionally with user software.  
**Find details in repository** [UPS-2_Raspberry_SW](https://github.com/ECOM-Klaus/UPS-2_Raspberry_SW.git)

