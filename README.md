# Low Pass Filter Design

## Project Overview

This project involves the design and implementation of a low-pass filter for a specific application, using both theoretical derivations and practical implementation techniques. The project follows a structured approach to achieve the desired filter characteristics, including simulation and prototype fabrication.

## Contents

- Introduction
- Design Guideline
- Design Target

## Introduction

### Type of Response

The passband ripple and the number of reactive elements are selected based on the preferred type of response:
1. **Butterworth response** (Maximally flat)
2. **Chebyshev response** (Equal ripple)
3. **Gaussian response**
4. **Elliptic function response**

## Filter Design by Insertion Loss Method

\[ \text{Insertion Loss (IL)} = 10 \log_{10} \left( \frac{\text{Power delivered to load}}{\text{Power available from source}} \right) \]

## Low-Pass Filter Prototype

The design begins with selecting an appropriate prototype for the low-pass filter, followed by the realization using microstrip or other suitable techniques.

## Design Guideline

### Example

Design a Chebyshev low-pass filter with the following specifications:
- Cutoff frequency: 2 GHz
- Equal ripple: 0.5 dB
- Rejection: -25 dB at \( f = f_c + 1 \text{ GHz} \)
- Filter impedance: 50 Ω (highest impedance: 100 Ω, lowest impedance: 30 Ω)
- Substrate: FR4
  - Thickness: 1 mm
  - Dielectric constant: 4.3

### Component Derivation

1. **Ideal Components Derivation**: Calculation of ideal inductor and capacitor values.
2. **Distributed Transmission Line Design**: Converting ideal values into practical microstrip components.
3. **Layout Realization**: Creating the layout for fabrication.

## Ideal Component Derivation

Two topologies are considered: starting with a series component or starting with a shunt component. The order of the filter is determined based on the given specifications.

## Simulation Results

Simulation results are used to verify the design, focusing on key parameters such as input return loss and insertion loss.

## Practical Implementation Issues

### Real Components vs Circuit Symbols

Real components have finite sizes and form factors, commonly in 1206, 0805, 0603, and 0402 packages. Practical issues include:
- Soldering
- PCB layout considerations
- Grounding through via holes
- Input/output connectors for testing
- Finite values for inductors and capacitors

### PCB Parameters

Substrate parameters for the design:
- Substrate thickness: 1 mm
- Relative dielectric constant: 4.34
- Conductor thickness: 0.02 mm
- Dielectric loss tangent: 0.025

## Simulation with Lumped Elements

The initial simulation uses ideal lumped elements. Practical implementation involves adjustments to account for real component values and layout constraints.

## Design Target

### Specification for Project

Design a low-pass filter with:
- 0.5 dB ripple
- 1.5 GHz cutoff frequency
- 50 Ω input/output impedance
- Rejection of -35 dB at \( f = f_c + 1.5 \text{ GHz} \)

### Selection of N

The order of the filter (N) is determined based on the given specifications. The filter order is checked and verified through simulations and practical considerations.

## Layout

The layout is created based on the derived components and specifications, ensuring that all practical implementation issues are addressed.

## Conclusion

This project provides a comprehensive approach to designing a low-pass filter, from theoretical derivations to practical implementation. The use of simulations and prototype fabrication ensures that the design meets the specified requirements.

---

Enjoy your work on the ASIC Designing Assistant!
