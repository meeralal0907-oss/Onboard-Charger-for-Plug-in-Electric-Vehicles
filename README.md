# Onboard Charger for Plug-in Electric Vehicles

## Project Overview

Designed and simulated a two-stage Onboard Charger (OBC) for plug-in electric vehicles using a Bridgeless Interleaved Boost Power Factor Correction (PFC) converter and a Phase-Shifted Full-Bridge (PSFB) converter. The project focuses on improved power quality, reduced switching losses, galvanic isolation and laboratory-scale hardware implementation.

## Why Onboard Charging?

Small electric vehicles, such as electric scooters and e-rickshaws, primarily depend on external chargers, limiting charging flexibility and compatibility with public charging infrastructure.

An onboard charger integrates the power conversion system within the vehicle, enabling direct AC charging without requiring a separate external charger.

The proposed architecture aims to overcome conventional charging limitations through improved power factor, reduced harmonic distortion and efficient power conversion.

## Objectives

- Design a compact two-stage onboard charging system.
- Achieve near-unity power factor.
- Minimize conduction and switching losses.
- Reduce input current ripple and harmonic distortion.
- Provide galvanic isolation for battery charging.
- Develop a laboratory-scale hardware prototype.

## System Architecture

AC Supply → EMI Filter → Bridgeless Interleaved Boost PFC → DC Link → Phase-Shifted Full-Bridge Converter → Battery

## Working Principle

### Stage 1: Bridgeless Interleaved Boost PFC Converter

- Converts AC input into regulated DC voltage.
- Eliminates the conventional diode bridge in the proposed topology to reduce conduction losses.
- Uses interleaved switching to minimize current ripple and distribute current stress.
- Employs PI-based control for power factor correction and voltage regulation.

### Stage 2: Phase-Shifted Full-Bridge Converter

- Performs isolated DC-DC power conversion.
- Uses phase-shifted PWM control to regulate power transfer.
- Employs Zero Voltage Switching (ZVS) to minimize switching losses.
- Provides galvanic isolation using a high-frequency transformer.
- Uses rectification and LC filtering to obtain a smooth DC output.

## Simulation and Results

The proposed converter stages were modelled and analysed using MATLAB/Simulink.

Key simulation outcomes include:

- Near-unity power factor.
- Regulated DC-link voltage.
- Stable DC-DC output voltage and current.
- Phase-shifted PWM switching waveforms.
- Soft-switching operation.

## Hardware Implementation

A laboratory-scale hardware prototype was developed to evaluate the practical feasibility of the proposed charger architecture.

The experimental setup incorporates a scaled AC supply, bridge rectification, Arduino-based PWM generation, MOSFET gate driver circuits, boost conversion and an isolated full-bridge DC-DC stage.

Hardware testing focused on voltage boosting, PWM signal generation, soft-switching waveforms and output voltage analysis.

## Hardware Components

| Component | Function |
|---|---|
| Arduino Uno | PWM signal generation |
| IR2110 | MOSFET gate driver |
| IRF540N | Power switching |
| MUR460 | Fast-recovery boost diode |
| KBPC3510 | Bridge rectification |
| LM2596 | Auxiliary power supply |
| Ferrite-core inductors | Energy storage and filtering |
| ETD34 transformer | Galvanic isolation and voltage conversion |
| Capacitors | DC-link stabilization and filtering |

## Tools and Technologies

- MATLAB/Simulink
- Arduino Uno
- Power Electronics
- AC-DC and DC-DC Converters
- Pulse Width Modulation (PWM)
- PI Control
- Power Factor Correction (PFC)
- Zero Voltage Switching (ZVS)
- MOSFET Gate Driver Circuits
- Hardware Prototyping and Testing

## Applications

- Electric scooters
- Electric two-wheelers
- E-rickshaws
- Compact plug-in electric vehicles

## Future Scope

- Full-power hardware validation.
- Thermal management optimization.
- Battery Management System (BMS) integration.
- EVSE communication and public charging compatibility.
- Closed-loop battery charging control.
- Experimental efficiency and THD evaluation.

## Conclusion

The project demonstrates the design, simulation and laboratory-scale hardware development of an onboard charging architecture for electric vehicles. The integration of power factor correction, interleaved switching, phase-shifted control and galvanic isolation provides a foundation for compact and efficient EV charging systems.

