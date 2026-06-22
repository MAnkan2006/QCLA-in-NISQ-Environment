# Quantum Carry Lookahead Adder (QCLA) in NISQ Environment

## Overview

This repository presents the implementation and performance evaluation of a **Quantum Carry Lookahead Adder (QCLA)** in a **Noisy Intermediate-Scale Quantum (NISQ)** environment using Qiskit.

The project investigates the impact of realistic quantum noise on the accuracy and reliability of QCLA circuits by simulating various noise models and analyzing their effects through quantitative error metrics. The study aims to evaluate the robustness of quantum arithmetic operations in near-term quantum devices.

---

## Objectives

- Implement a Quantum Carry Lookahead Adder (QCLA) using Qiskit.
- Simulate the circuit under ideal and noisy quantum environments.
- Analyze the impact of different quantum noise models.
- Evaluate circuit performance using standard error metrics.
- Compare the behavior of QCLA in ideal and NISQ settings.

---

## Key Features

- Quantum Carry Lookahead Adder (QCLA) implementation.
- NISQ-aware quantum simulation.
- Support for multiple quantum noise models:
  - Bit Flip Noise
  - Phase Flip Noise
  - Depolarizing Noise

- Ideal vs Noisy execution comparison.
- Error analysis using:
  - Error Rate (ER)
  - Normalized Mean Error Distance (NMED)
  - Mean Relative Error Distance (MRED)

- Visualization of experimental results.

---

## Background

The Quantum Carry Lookahead Adder (QCLA) is a quantum arithmetic circuit designed to reduce carry propagation delay by generating and propagating carry information in parallel.

Compared to Ripple Carry Adders, QCLA achieves lower circuit depth and improved computational efficiency, making it a promising architecture for large-scale quantum arithmetic operations.

However, the increased gate complexity and qubit interactions make QCLA susceptible to noise in NISQ devices. This project studies these effects through extensive simulation.

---

## Technologies Used

- Python
- Qiskit
- Qiskit Aer
- NumPy
- Matplotlib
- IBM Quantum Platform

---

## Methodology

### 1. Circuit Construction

The QCLA circuit is constructed using reversible quantum gates such as:

- CNOT Gate
- Toffoli Gate (CCX)
- X Gate

### 2. Input Encoding

Classical binary operands are encoded into quantum states.

### 3. Ideal Simulation

The circuit is executed on an ideal simulator to obtain reference outputs.

### 4. Noise Injection

Different noise models are applied to emulate realistic NISQ hardware behavior.

### 5. Performance Evaluation

Simulation outputs are compared against expected outputs using quantitative error metrics.

---

## Noise Models

### Bit Flip Noise

Models unintended flips between quantum states:

|0⟩ ↔ |1⟩

---

### Phase Flip Noise

Introduces phase errors while preserving measurement probabilities:

|1⟩ → −|1⟩

---

### Depolarizing Noise

Randomly applies Pauli operations:

- X
- Y
- Z

with a specified probability.

---

## Error Metrics

### Error Rate (ER)

Measures the fraction of incorrect outputs produced by the noisy circuit.

[
ER = \frac{\text{Number of Incorrect Outputs}}{\text{Total Outputs}}
]

---

### Normalized Mean Error Distance (NMED)

Measures the average deviation of noisy outputs from expected outputs, normalized by the maximum output range.

---

### Mean Relative Error Distance (MRED)

Measures the relative computational error compared to the correct output.

---

## Experimental Workflow

1. Generate QCLA quantum circuit.
2. Encode binary inputs.
3. Execute ideal simulation.
4. Apply selected noise model.
5. Execute noisy simulation.
6. Collect measurement outcomes.
7. Compute ER, NMED, and MRED.
8. Analyze performance degradation.

---

## Results

The impact of different noise models is evaluated through extensive simulations.

| Noise Model | Error Rate (ER) | NMED  | MRED  |
| ----------- | --------------- | ----- | ----- |
| Ideal       | 0.000           | 0.000 | 0.000 |

| Depolarizing | 52.46 | 0.120 | 0.352 |
| Bit Flip | 88.93 % | 0.225 | 0.651 |
| Phase Flip | Experimental | Experimental | Experimental |

Replace the above values with the actual results obtained from simulations.

---

## Applications

- Quantum Arithmetic Circuits
- Quantum Algorithm Design
- NISQ Benchmarking
- Quantum Error Analysis
- Quantum Computer Architecture
- Fault-Tolerant Quantum Computing Research

---

## Future Work

- Larger-bit QCLA implementations.
- Execution on real IBM Quantum hardware.
- Error mitigation and correction techniques.
- Hardware-aware circuit optimization.
- Comparative studies with:
  - Quantum Ripple Carry Adder (QRCA)
  - Vedral-Barenco-Ekert Adder
  - Thapliyal Adder

---

## Installation

Clone the repository:

```bash
git clone https://github.com/MAnkan2006/QCLA-in-NISQ-Environment.git
cd QCLA-in-NISQ-Environment
```

Install dependencies:

```bash
pip install qiskit qiskit-aer numpy matplotlib
```

---

## Usage

Run the simulation notebooks or Python scripts included in the repository.

Example:

```bash
python qcla.py
```

The program will:

- Construct the QCLA circuit.
- Simulate ideal execution.
- Simulate noisy execution.
- Compute ER, NMED, and MRED metrics.
- Generate comparative performance results.

---

## Repository Structure

- QCLA Circuit Implementation
- Noise Model Simulations
- Error Metric Evaluation
- Experimental Results
- Visualization and Analysis
- Documentation

---

## Author

**Ankan Mandal**

B.Tech, Computer Science and Engineering
National Institute of Technology Durgapur

GitHub: https://github.com/MAnkan2006

---

## Citation

If you use this work in your research, please cite:

```text
Ankan Mandal.
"Quantum Carry Lookahead Adder (QCLA) in NISQ Environment."
GitHub Repository, 2026.
```

---
