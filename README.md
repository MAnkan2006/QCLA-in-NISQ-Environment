# QCLA in NISQ Environment

## Overview

This repository explores a **Quantum Carry Look-Ahead Adder (QCLA)** in a **Noisy Intermediate-Scale Quantum (NISQ)** environment.

The project is organized as a set of Jupyter notebooks that study how the adder behaves under different noise models, with a focus on practical quantum-circuit simulation.

## Repository Contents

The repository currently includes:

- `ThapliyalAdderBitflipNoiseModel.ipynb`
- `ThapliyalAdderDepolarisingNoiseModel.ipynb`
- `ThapliyalAdderPhaseNoiseModel.ipynb`

Each notebook investigates the same adder design under a different noise model.

## Noise Models Studied

- **Bit-flip noise**
- **Depolarising noise**
- **Phase noise**

These experiments help compare how the adder behaves when the quantum circuit is affected by different kinds of errors that are common in NISQ-era hardware.

## How to Use

1. Open the repository in **Jupyter Notebook** or **JupyterLab**.
2. Run the notebook you want to inspect.
3. Execute the cells from top to bottom to reproduce the simulation and analysis.
4. Compare the outputs across the three noise-model notebooks.

## Suggested Workflow

For each notebook:

1. Define the adder circuit.
2. Set up the selected noise model.
3. Run the circuit simulation.
4. Measure the output distribution.
5. Compare the observed results across noise settings.

## Project Structure

```text
.
├── README.md
├── ThapliyalAdderBitflipNoiseModel.ipynb
├── ThapliyalAdderDepolarisingNoiseModel.ipynb
└── ThapliyalAdderPhaseNoiseModel.ipynb
```

## Notes

- The repository is notebook-based.
- The current focus is on experimenting with QCLA under different noisy conditions.
- If additional scripts, datasets, or dependencies are added later, they can be documented here.


