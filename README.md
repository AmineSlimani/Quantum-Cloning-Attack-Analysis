# Quantum Cloning Attack Analysis

![GitHub](https://img.shields.io/badge/license-MIT-blue) 
![Python](https://img.shields.io/badge/Python-3.7%2B-blue)

This repository contains a Python-based analysis of mutual information in the context of a **quantum cloning attack**. The project explores the relationship between Alice, Bob, and Eve in a quantum communication scenario, focusing on mutual information measures and their dependence on the probability of error.

## Table of Contents
- [Overview](#overview)
- [Key Concepts](#key-concepts)
- [Repository Structure](#repository-structure)
- [Requirements](#requirements)
- [Usage](#usage)
- [Results](#results)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Overview

In quantum cryptography, a **cloning attack** is an attempt by an eavesdropper (Eve) to clone the quantum states sent by Alice to Bob. This project analyzes the mutual information between the parties involved and how it changes with the probability of error (\(P_{error}\)). The analysis is performed using Python, with visualizations generated using Matplotlib.

The notebook calculates and plots the following mutual information measures:
- \(I_{AB}\): Mutual information between Alice and Bob.
- \(I_{AE}\): Mutual information between Alice and Eve.
- \(I_{BSE}\): Mutual information of Bob superior to Eve.

---

## Key Concepts

### Mutual Information
- **\(I_{AB}\)**: Measures the correlation between Alice and Bob's shared quantum states.
- **\(I_{AE}\)**: Measures the correlation between Alice and Eve's cloned quantum states.
- **\(I_{BSE}\)**: Represents the advantage Bob has over Eve in terms of mutual information.

### Probability of Error (\(P_{error}\))
The probability that Bob's measurement result differs from Alice's sent state. It is calculated as:
\[
P_{error} = \frac{1 - \cos(\theta)}{2}
\]
where \(\theta\) is the angle between quantum states.

---


---

## Requirements

To run the code in this repository, you need the following Python packages:
- **NumPy**: For numerical calculations.
- **Matplotlib**: For plotting the results.

You can install the required packages using the following command:
```bash
pip install numpy matplotlib
