## Summary of the Fundamentals of VSDBabySoC

## Overview
This project is focused on creating a small, open-source System on Chip (SoC) called BabySoC, which includes the RVMYTH, a RISC-V processor core.
The SoC contains two vital parts — a Phase-Locked Loop (PLL) that helps generate synchronized and accurate clock signals, and a 10-bit Digital-to-Analog Converter (DAC) that handles the conversion of digital data to analog signals. With these components, BabySoC can connect to analog devices such as televisions and mobile phones to produce audio or video signals. The project uses Sky130 technology to build it, making it a useful tool for learning and experimenting with digital-to-analog interfacing.

## SoC Basics
A System on Chip (SoC) is like a complete computer built on a single chip.
It includes elements like a CPU, memory, input/output ports, GPU, DSP, and power management units. SoCs are found in many devices, such as smartphones, tablets, IoT devices, and smart appliances, due to their compact size, high performance, energy efficiency, and cost-effectiveness. However, designing them is complex and can lead to challenges like heat issues and limited flexibility.

## There are three main types of SoCs:

- Microcontroller-based SoCs: Used for simple control tasks in low-power devices.

- Microprocessor-based SoCs: Designed for multitasking and running operating systems in devices like smartphones.

- Application-Specific SoCs: Built for specialized high-end applications like AI, graphics, or networking.


## VSDBabySoC includes three important open-source IP cores:

- RVMYTH (RISC-V Processor): Acts as the core that processes data and instructions.
It uses register r17 to store data that the DAC will use.
- Phase-Locked Loop (PLL): Generates a stable clock signal to ensure all components work in sync, which is vital for timing and system stability.

- Digital-to-Analog Converter (DAC): Converts digital data from the RVMYTH into an analog signal that can be sent to external devices for audio or video output.


In practice, BabySoC starts by using the PLL to create a synchronized clock signal.
The RVMYTH processor handles digital data and updates its registers, which are then turned into an analog wave by the DAC. The final output is saved in a file named OUT and can be connected to external analog systems, demonstrating actual digital-to-analog conversion.

The PLL works by matching the phase and frequency of its output signal to a reference input signal.
It has three key parts — a Phase Detector, Loop Filter, and Voltage-Controlled Oscillator (VCO). Using on-chip PLLs avoids issues like clock delays, jitter, and frequency mismatches that arise with external clock sources.

## The DAC changes digital binary values into continuous analog voltages.
Two common types are:

- Weighted Resistor DAC
- R-2R Ladder DAC
BabySoC uses a 10-bit R-2R Ladder DAC to create 1024 different analog levels.


In summary, the VSDBabySoC project merges digital computation with analog interfacing in a small package.
It not only shows how SoCs operate but also provides a hands-on learning platform to explore RISC-V cores, PLL-based clock management, and DAC-based analog conversion in a single open-source chip.
