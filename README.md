# Adjustable DC Power Supply Unit (1.2V - 30V)

![Status](https://img.shields.io/badge/Status-Prototype-yellow)
![Tool](https://img.shields.io/badge/Tool-Proteus%208-blue)
![Hardware](https://img.shields.io/badge/Hardware-PCB%20%2F%20Breadboard-green)

## Project Overview
This project involves the design, simulation, and prototyping of a robust dual-output DC power supply unit. The system is designed to provide a **fixed 12V output** for auxiliary cooling and a generic **adjustable output (1.2V - 30V)** for laboratory bench use.

The circuit utilizes the **LM338T** linear voltage regulator for high-current adjustable output and the **L7812** for stable fixed voltage, ensuring reliability under load with integrated thermal management.

## Key Features
* **Dual Output Architecture:**
  * Output 1: Fixed **12V DC** (via L7812CV)
  * Output 2: Adjustable **1.2V - 30V DC** (via LM338T)
* **High Current Capability:** Designed to handle loads up to 5A with proper heatsinking.
* **Thermal Protection:** Integrated heatsinks and active cooling fan (12V) for continuous operation.
* **Real-time Monitoring:** Digital Panel Meter for simultaneous voltage and current display.
* **Safety:** AC input fused protection and diode-based reverse current protection.

## Technical Specifications
| Parameter | Value |
| **Input Voltage** | 220V AC (Transformer Primary) |
| **Transformer Output** | 24V AC / 100VA |
| **Rectification** | Full-Wave Bridge (KBPC3510 - 35A) |
| **Adjustable Regulator** | LM338T (1.2V - 32V Range) |
| **Fixed Regulator** | L7812CV (12V) |
| **Filter Capacitance** | 4700µF (Electrolytic) |

## Project Gallery

### 1. Circuit Schematic (Proteus)
The circuit was designed and simulated in Proteus Design Suite.
![Circuit Diagram](schematics/circuit_diagram.png)

### 2. AC Input Stage & Rectification
High-power AC/DC conversion stage featuring a 100VA transformer and KBPC3510 bridge rectifier.
![Transformer Assembly](schematics/transformer_rectifier_assembly.jpg)

### 3. Prototype Assembly (Breadboard)
Initial build for voltage verification, thermal testing, and load regulation analysis.
![Breadboard Prototype](schematics/breadboard_setup.jpg)

## Documentation
* **[Bill of Materials (BOM)](docs/Bill_of_Materials.pdf):** Detailed list of all components used in this project.
* **Datasheets:** Technical references for key components can be found in the `docs/` folder.

## Simulation
The simulation files are located in the `simulation/` directory. You can run the `.pdsprj` file using **Proteus 9**.

---
*Author: [Halil Alperen Nisevci]*
