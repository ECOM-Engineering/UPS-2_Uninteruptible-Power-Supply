

# USER MANUAL

# UPS-2 Uninterruptible Power Supply 

## Hat Solution For Raspberry Pi Computers

UPS-2 is a wide input range, high efficiency power supply for Raspberry Pi computers. It features a main input and a backup input. In case of power fail or under voltage at the main input,  backup input becomes active  with no interruption or spike on the Raspberry 5V, 3A supply output.   
Firmware provides optical and software state feedback, including voltage levels, warnings and CPU temperature.  
UPS-2 can be controlled by software commands from the Raspberry and/or by the on board  push button. Supply commands include POWER OFF, STANDBY and RESTART. 

- Compatible with Raspberry models 3, 3B, 4B and zero W
- High efficiency power supply with output 5V, 3A
- Main input voltage range 8V ... 18V
- Shutdown function with real power-off  
- Battery standby current < 20uA @9V
- Battery voltage 6.5V ... 18V
- Nearly no self heating thanks to outstanding conversion efficiency
- Communication with Pi via serial UART or parallel port
- Python library for unattended operation and optional GUI



## Functions

### Hardware Control

#### Power Input Section

| Input                     | Selection                   | Remark                             |
| :------------------------ | --------------------------- | ---------------------------------- |
| Main                      | Selected if > 8V            | Independent of battery voltage     |
| Battery                   | Selected if main input < 7V | Battery voltage > 6.5V             |
| Raspberry USB power input | Selected if present         | Priority over Main and Batt inputs |

#### LED Indicators

| Input Voltage    | White LED: Main | Blue LED: Battery |
| ---------------- | --------------- | ----------------- |
| Voltage in range | ON              | ON                |
| Voltage low      | BLINK           | BLINK             |
| No input         | OFF             | OFF               |



| Raspberry State     | Green LED *) | Raspberry Red LED |
| ------------------- | ------------ | ----------------- |
| Complete power OFF  | OFF          | OFF               |
| Standby (shut down) | OFF          | ON                |
| Starting up         | BLINK FAST   | ON                |
| Run (up)            | ON           | ON                |
| Shutting down       | BLINK SLOW   | ON                |

*) Green LED shows also feedback at push button operation 



#### Push Button Operations

Push button allows manual invocation of different shut down and start up functions.

| Button Operation | Function                  | Green LED                |
| ---------------- | ------------------------- | ------------------------ |
| Short press      | Start up from power off   | fast blink               |
| > 2 seconds      | Shutdown to standby *)    | > 2 blinks               |
| > 5 seconds      | Shutdown to power off **) | > 5 blinks               |
| Double click     | Shutdown and restart      | slow blink -> fast blink |



## Hardware Connections

#### UPS-2 Hat <> Raspberry-Pi Connections



<figure>
  <img
  src="../images/Connections.png" 
  alt="UPS-2 Hat connections">
  <figcaption>UPS-2 Hat connections</figcaption>
</figure>





## Quick Start








## GUI-Graphical User Interface

Hyperlink to figure



## Software API



## Technical Data