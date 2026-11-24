# Hybrid Energy Storage System: Battery and Supercapacitor

This repository contains the firmware developed using MPLAB X IDE, the Altium Designer PCB design files, and the PLECS simulation model for a hybrid energy storage system (HESS) combining a battery and a supercapacitor at the cell level.

## MPLAB IDE firmware

The microcontroller firmware was developed using MPLAB X IDE and is provided in the following compressed archive:

- `HIBRIDATION_SC_BATT.rar`

The firmware implements the control and monitoring functions required for the experimental HESS prototype, including ADC measurements, PWM signal generation, operating-state management, and the control algorithms used to regulate the converter.

To explore or modify the firmware:

1. Extract the HIBRIDATION_SC_BATT.rar archive.
2. Open MPLAB X IDE and load the extracted project.
3. Review the microcontroller configuration, peripheral settings, and control parameters.
4. Build the project using the appropriate compiler and device configuration.
5. Program the microcontroller using a compatible programming or debugging interface.

Before programming the hardware, verify the PWM configuration, ADC channel assignments, control parameters, and protection thresholds to ensure compatibility with the experimental prototype.

## PCB Design

The Altium project includes:

- **PCB_Project.PrjPcb**: main project file.
- **PCB1.PcbDoc**: printed circuit board layout.
- **CURRENT_SENSE.SchDoc**: current sensing circuit.
- **DRIVER_2.SchDoc**: driver circuit.
- **DRIVER_ADN_REGULATORS.SchDoc**: drivers and power supply regulators.
- **MCU.SchDoc**: microcontroller circuit.
- **MOSFET_AND_INTRUMENTAL_AMPLIFIERS.SchDoc**: MOSFET stage and instrumentation amplifiers.
- **PCB_Project.BomDoc**: bill of materials document.
- **PCB_Project.OutJob**: configuration for generating documentation and output files.
- **PCB_Project.pdf**: exported documentation for reference.

To explore or edit the design, open `PCB_Project.PrjPcb` in Altium Designer.

## PLECS Simulations

Simulation models are included to study the hybrid energy storage topology:

- `HESS_ARTICLE_TOPOLOGY_1.plecs`

Open this file in PLECS to explore and run the model. Review its parameters, initial conditions, and control signals before running a simulation.

## Requirements

- **MPLAB X IDE** to open, modify, and build the microcontroller firmware.
- Compatible compiler and programming tools to compile and program the microcontroller.
- **RAR extraction software** to extract the firmware project.
- **Altium Designer** to open and edit the schematic and PCB files.
- **PLECS** to open and run the simulation models.
- A PDF reader to view the exported documentation.

## Notes

The Altium project references the external libraries `SamacSys.PcbLib` and `SamacSys.SchLib`. If these libraries are not included in the repository, they must be provided separately or their paths updated to work with them.

Altium history folders, backup files, and temporary logs are excluded to keep the repository focused on the design files.

Before manufacturing the PCB, verify the design rules, connections, component footprints, and manufacturing outputs. Review the simulation models against the intended operating conditions.
