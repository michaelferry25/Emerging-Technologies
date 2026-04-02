# Emerging Technologies Assessment

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![Qiskit](https://img.shields.io/badge/qiskit-latest-6929C4?logo=ibm&logoColor=white)
![Qiskit Aer](https://img.shields.io/badge/qiskit--aer-latest-blueviolet?logo=ibm&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-latest-013243?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/matplotlib-latest-11557c)
![Jupyter](https://img.shields.io/badge/jupyter-latest-F37626?logo=jupyter&logoColor=white)

**Author:** Michael Ferry  
**Module:** Emerging Technologies  
**Year:** 2026

## Overview

This repository contains solutions to quantum computing problems exploring the Deutsch-Jozsa algorithm. The assessment demonstrates the difference between classical and quantum approaches to determining whether Boolean functions are constant or balanced.

## Repository Structure
```
Emerging-Technologies/
├── problems.ipynb          # Main Jupyter notebook with all solutions
├── requirements.txt        # Python package dependencies
├── README.md              # This file
└── .gitignore            # Git ignore rules
```

## Problems Covered

### Problem 1: Generating Random Boolean Functions
Implementation of a function that generates random constant or balanced Boolean functions with four inputs. Uses lookup tables to store all possible input-output mappings.

### Problem 2: Classical Testing for Function Type
Classical algorithm to determine if a function is constant or balanced. Demonstrates that up to 9 queries are needed in the worst case to be certain.

### Problem 3: Quantum Oracles
Implementation of quantum oracles for all four possible single-bit Boolean functions using Qiskit:
- f(x) = 0 (constant)
- f(x) = 1 (constant)
- f(x) = x (balanced, identity)
- f(x) = NOT x (balanced, negation)

### Problem 4: Deutsch's Algorithm
Quantum circuit implementation of Deutsch's algorithm using the oracles from Problem 3.

### Problem 5: Deutsch-Jozsa Algorithm 
Scaling Deutsch's algorithm to handle four-bit Boolean functions.

## Setup

Clone the repository and install dependencies:
```bash
git clone https://github.com/michaelferry25/Emerging-Technologies.git
cd Emerging-Technologies
pip install -r requirements.txt
jupyter notebook problems.ipynb
```

## Dependencies

- Python 3.8+
- NumPy
- Qiskit
- Qiskit-Aer
- Matplotlib

See `requirements.txt` for complete list with versions.

## Key Concepts

**Quantum Advantage:** The Deutsch-Jozsa algorithm demonstrates exponential speedup over classical algorithms. Where classical algorithms need O(2^(n-1) + 1) queries, the quantum approach needs only 1.

**Superposition:** Quantum bits can exist in multiple states simultaneously, allowing parallel evaluation of multiple inputs.

**Interference:** Quantum gates create interference patterns that encode the global properties of functions.

## Author

Michael Ferry, Student at ATU Galway City
