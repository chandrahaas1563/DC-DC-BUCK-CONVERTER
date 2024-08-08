## DC-DC Buck Converter
### Project Overview
This project involves the design and hardware implementation of a Buck Converter using the TL494 PWM generator IC. This was a group project that was done in the Power Electronics Course.
### Problem Statement
Design a Buck Converter with the following specifications:
* Input Voltage: 15 V
* Output Voltage: 10 V
* Switching Frequency: 10 kHz
* Output Current: 1 A

The project includes generating waveforms of inductor current and switch voltage in Continuous Conduction Mode (CCM) and demonstrating Discontinuous Conduction Mode (DCM) by changing the load resistance.
### Components and Equipment
* Drive Circuit (TL494 PWM generator IC ): Generates the pulse width modulated signal to control the transistor.
* MOSFET: Acts as a high-speed switch controlled by the PWM.
* Diode: Provides a path for the inductor current when the switch is off.
* Inductor: Stores energy and helps in smoothing the current.
* Capacitors: Filters the output to reduce voltage ripple.
* Resistors: Used for sensing and feedback purposes.
* MOSFET driver: To connect the TL494 board and drive circuit.
* Rheostat: To change load resistance.
* Oscilloscope: To observe waveforms.
### Key Concepts
#### Continuous Conduction Mode (CCM)
CCM occurs when the current through the inductor never falls to zero during the switching cycle. This mode is characterized by continuous current flow in the inductor.
#### Discontinuous Conduction Mode (DCM)
DCM occurs when the current through the inductor falls to zero during part of the switching cycle. This mode is characterized by intermittent current flow in the inductor.
### Circuit Design
#### TL494 PWM generator IC
The TL494 board generates the pulses for the DC-DC PE converters. Here is the connection diagram for the same:
IMAGE
#### Interface circuit to driver IC
This connects the driver IC to the output obtained from the TL494 board. The circuit diagram for the same is shown below. 
IMAGE
#### Buck Converter Circuit
A Buck Converter, or a step-down converter, is a DC-DC converter that steps down the voltage from its input to its output. 
IMAGE
### Implementation Steps
* **Circuit Design**: Design the circuit according to the specifications. Ensure that the components are rated for the required voltages and currents.
* **Component Selection**: Select appropriate components such as MOSFETs, diodes, inductors, and capacitors.
* **PCB Layout**: Design the PCB layout to ensure minimal noise and optimal performance.
* **Assembly**: Assemble the circuit components on the PCB.
* **Testing**: Test the circuit under various load conditions to verify performance in both CCM and DCM.
### Waveforms and Analysis
* **Gate Pulses**: The gate pulse (PWM output) waveform is shown in yellow.
* **Inductor Current & Switch Voltage**: The inductor Current & switch voltage is shown in blue.
#### Waveforms in CCM
* 



