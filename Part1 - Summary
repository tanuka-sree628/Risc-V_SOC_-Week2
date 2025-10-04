## Summary of the fundamentals of VSDBabySoc

This work aims to develop a small, open-source System on Chip (SoC) known as BabySoC, with the RVMYTH, which is a RISC-V processor core. The SoC contains two important components — a Phase-Locked Loop (PLL) used for synchronous and accurate clock generation and a 10-bit Digital-to-Analog Converter (DAC) used for digital to analog conversion.
By doing the above, BabySoC will be able to interface with analog devices like televisions and cell phones to generate audio or video signals. Using Sky130 technology to implement it, this project hopes to be an educational and experimental vehicle to learn digital–analog interfacing.

System on Chip (SoC) is literally a computer in its entirety fabricated on a single chip. It has elements such as a CPU, memory, I/O ports, GPU, DSP, and power management units. SoCs are omnipresent in smartphones, tablets, IoT devices, and smart appliances because they are compact in size, high-performance, energy efficient, and economical. But they are difficult to design, and they can suffer from issues such as heat dissipation and lack of flexibility.

## There are three principal categories of SoCs:

Microcontroller-based SoCs – applied to straightforward control applications and low-power devices.

Microprocessor-based SoCs – targeted to multitasking as well as the execution of operating systems on devices such as smartphones.

Application-Specific SoCs – constructed for high-end specialized applications like AI, graphics, or networking.

## VSDBabySoC incorporates three significant open-source IP cores:

RVMYTH (RISC-V Processor): Serves as the processing core, executing data and instructions. It utilizes register r17 as a holding area for values for the DAC.

Phase-Locked Loop (PLL): Produces a stable clock signal to synchronize all the components for appropriate timing and system stability.

Digital-to-Analog Converter (DAC): Converts the digital data from RVMYTH to an analog signal that can be transmitted to external devices for audio or video output.

In practice, BabySoC commences operation by the PLL producing a synchronized clock. The RVMYTH processor handles digital information and refreshes its register, which is then converted to an analog wave by the DAC. The output, saved in a file called OUT, can be interfaced to external analog systems, showing actual digital-to-analog conversion.

The PLL itself operates by synchronizing the phase and frequency of its output signal to a reference input signal. It consists of three essential components — a Phase Detector, Loop Filter, and Voltage-Controlled Oscillator (VCO). Utilizing on-chip PLLs prevents clock delays, jitter, and frequency mismatches that occur when utilizing external clock sources.

## The DAC also converts digital binary values to continuous analog voltages. Two popular ones are:

Weighted Resistor DAC

R-2R Ladder DAC
The 10-bit R-2R Ladder DAC is implemented in BabySoC to deliver 1024 discrete analog levels.

All in all, the VSDBabySoC project integrates digital computation with analog interfacing in small size. Not only does it demonstrate how SoCs work, but it also offers a hands-on, learning platform for experiencing the integration of RISC-V cores, PLL-based clock domains, and DAC-based analog conversion in one open-source chip.
