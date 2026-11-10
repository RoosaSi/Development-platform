# DEVELOPMENT PLATFORM
STM32-based development platform. Includes display, programmable buttons, buzzer and GPIO-pins. Power is through USB-C.

**Project overview:** 
The objective of this project was to design and implement a microcontroller-based development platform for programming practice

**Key features:** 
Microcontroller: STM32F411RCT6. It features a 32-bit Arm Cortex-M4 core running up to 100MHz. It has several features that make it suitable for embedded systems development, peripheral interfacing, sensor data acquisition and real-time control applications. For example it has 256 KB of Flash memory, 128 KB of SRAM, a 12-bit ADC, general-purpose timers, and communication peripherals such as UART, SPI, I²C, and USB Full-Speed OTG.

Power supply: Adafruit USB type C breakout board and voltage regulator to adjust voltage to 3.3V. All components were chosen to work at same voltage as microcontroller. USB connectivity was only used for power. Maybe in new iterations of the PCB it could also be used for data. 

GPIO expansion: 2x16 GPIO pins for development. Allows for UART/SPI/I2C communication with external sensors etc.

Reset-button

Status LED: indicates when power is on

Display Module: Waveshar 2inch LCD Display Module, uses SPI interface. 

**PCB design:** 
The platform was designed using Altium Designer. It has 2 layers and the dimensions are 13,7cm x 17,6cm.

**Testing and validation:**
The PCB was inspected and tested using a digital multimeter to verify basic electrical connections and power distribution. I measured the supply voltages at relevant points on the PCB to confirm correct voltage levels. Also checked the continuity of data lines to verify that signals were routed to their intended connections. During checks I was happy with the routing. 
SWD interface was tested to verify connectivity with the microcontroller. This was done with simple code to ring the buzzer and use the buttons on the PCB. The test was succesful and confirmed that the SWD interface was correctly connected and accessible for debug and programming. 

**Results and lessons learned:** 
The result was an operational development platform. This project strengthened my understanding of what goes into designing a PCB. 
I improved my skills in schematic design, component placement and PCB routing and power distribution. I learned to select suitable components based on datasheets and electrical requirements. I also gained practical experience in soldering and assembling electronic components. 

Most importantly I learned the importance of systematic design, simulation and testing.

**Current project status:** 
Hardware design and testing is completed. Future work will include firmware development and practical experiments with the platform's peripherals and communication interfaces. 


### SCHEMATIC
[View full schematic (PDF)](https://github.com/RoosaSi/Development-platform/blob/main/Development_platform_schematic.pdf)

### LAYOUT
[View full layout (PDF)](https://github.com/RoosaSi/Development-platform/blob/main/Development_platform_layout.pdf)

