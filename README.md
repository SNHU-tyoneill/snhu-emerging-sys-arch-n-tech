# snhu-emerging-sys-arch-n-tech
SNHU Emerging Sys Arch &amp; Tech Portfolio

## Overview
This repository contains two projects developed during the course. These projects showcase my ability to write interface software to control hardware components, analyze hardware architecture design considerations, and recommend emerging technologies based on business requirements.

### Project 1: SOS/OK Prototype

#### Summary
This project involved developing a system that outputs Morse code signals for SOS and OK using GPIOs and timers on the TI board. The goal was to create a reliable way to signal distress (SOS) and confirmation (OK) using LED flashes, demonstrating low-level hardware control and communication protocol implementation.

#### What Went Well
I efficiently used timers to control the timing of the LED flashes, ensuring precise intervals mathcing Morse code requirements. Additionally, I structured the code to be modular, making it easy to adapt and expand to other signal patterns.

#### Improvement Areas
While the system worked as intended, I could have further optimized the code for better performance, particularly by minimizing the CPU usage during LED control operations. Implementing a more efficient sleep mode could have reduced power consumption. Another area is the amount of STATES used, this may have been simplified resulting in a more human readable and adaptable code base.

### Tools and Resources
- TI Code Composer Studio (CCS)
- TI CC3220x LAUNCHXL Development Board
- GPIO and Timer Peripherals

#### Transferable Skills
This project honed my skills in hardware-software integration, low-level peripheral control, and timing management, which are essential for embedded systems development and real-time applications.

#### Code Maintainability
I made the code maintainable, readable, and adaptable by implementing modular functions for each key operation (timer setup, LED control). The use of descriptive comments and naming conventions ensures that the project can be easily understood and modified.

### Project 2: Smart Thermostat Prototype

#### Summary
This project involved creating a smart thermostat prototype using the TMP006 terperature sensor to read the room temperature and an LED to simulate the heating system. Buttons were used to adjust the temperature setpoint, and data was communicated over UART to simulate server communication. The aim was to showcase the prototype functionaliity for a low-level thermostat system.

#### What Went Well
I successfully integrated multiple peripherals (I2C, GPIO, UART) and developed a task scheduler to manage the periodic reading of temperature, adjusting the setpoint, and reporting data to the UART console. The system was reliable and accurately adjusted the LED state based on temperature readings.

#### Improvement Areas
One area of improvement could be the optimization of the task scheduler to handle more complex tasks and additional peripherals with less CPU overhead. Additionally, further testing and calibration of the temperature sensor readings could improve accuracy.

#### Tools and Resources
- TI Code Composer Studio
- TI CC3220x LAUNCHXL Development Board
- TMP006 Temperature Sensor
- UART, I2C, GPIO Peripherals

#### Transferable Skills
The skills developed in this project, such as integrating multiple peripherals, managing interrupts, and creating a task scheduler, are highly transferable to future projects involving embedded systems, IoT devices, and real-time contorl systems.

#### Code Maintainability
I ensured the code was maintainable and readable by using consisten formatting, clear comments, and modular functions for each operation (temperature reading, LED control, UART communcation). The task scheduler was designed to be adaptable, allowing for additional tasks and peripherals to be easily integrated.
