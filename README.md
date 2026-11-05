# Hybrid Energy Storage System: Battery and Supercapacitor

This repository contains the Altium Designer PCB design files and PLECS simulation models for a hybrid energy storage system combining a battery and a supercapacitor.

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

Three simulation models are included to study different hybrid energy storage topologies:

- `HESS_ARTICLE_TOPOLOGY_1.plecs`
- `HESS_ARTICLE_TOPOLOGY_2.plecs`
- `HESS_ARTICLE_TOPOLOGY_3.plecs`

Open each file in PLECS to explore and run the model. Review its parameters, initial conditions, and control signals before running a simulation.

## Requirements

- **Altium Designer** to open and edit the schematic and PCB files.
- **PLECS** to open and run the simulation models.
- A PDF reader to view the exported documentation.

## Notes

The Altium project references the external libraries `SamacSys.PcbLib` and `SamacSys.SchLib`. If these libraries are not included in the repository, they must be provided separately or their paths updated to work with them.

Altium history folders, backup files, and temporary logs are excluded to keep the repository focused on the design files.

Before manufacturing the PCB, verify the design rules, connections, component footprints, and manufacturing outputs. Review the simulation models against the intended operating conditions.
