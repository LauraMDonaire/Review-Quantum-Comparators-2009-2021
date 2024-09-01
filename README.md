# Quantum Comparators

## Overview

This repository contains a collection of quantum comparator circuits along with an in-depth study of their performance. Developed as part of my Final Degree Project (TFG) titled **"Efficient Design of Quantum Circuit Comparators"**, this work aims to provide quantum circuit designers with the tools and analysis they need to select the most suitable comparator based on specific performance metrics.


## Introduction to Quantum Comparators

### What is a Quantum Comparator?

In classical computing, comparators are circuits used to compare two values and determine their relationship (e.g., whether one is greater than, less than, or equal to the other). In quantum computing, comparators perform a similar function but leverage quantum principles to achieve potentially more efficient or powerful comparisons.

A **quantum comparator** is a quantum circuit designed to compare quantum states or quantum bits (qubits). Unlike classical comparators, which operate on bits with definite values, quantum comparators work with superpositions and entanglements, allowing for more complex and potentially more efficient comparison operations.

### Importance of Quantum Comparators

Quantum comparators are crucial in various quantum algorithms and protocols. They can be used in quantum search algorithms, quantum sorting, and other quantum computational tasks where comparing quantum states or processing quantum information is required. Efficient quantum comparators can lead to improved performance in quantum algorithms, impacting overall quantum computation efficiency.

### Types of Quantum Comparators

Quantum comparators can be classified into three main types:

#### 1. Simple Comparator

A **simple comparator** checks whether two values, A and B, are equal or not. These comparators are relatively straightforward and can be easily implemented by comparing each bit of the values one by one.

#### 2. Medium Comparator

A **medium comparator** determines whether one value A is greater than or equal to another value B (i.e., A ≥ B). This type of comparator goes beyond mere equality and is useful in scenarios where a more nuanced comparison is required.

#### 3. Full Comparator

A **full comparator** performs a more comprehensive comparison by checking whether A is greater than B, equal to B, or less than B (i.e., A > B, A = B, or A < B). This type of comparator provides a complete comparison of the two values and is used when detailed relational information is needed.

In this work, we focus on medium comparators, which are currently useful in quantum computing due to their ease of integration with algorithms such as Grover's algorithm.

## Motivation

The motivation behind this project is to address the growing need for efficient quantum circuits as quantum computing continues to advance. By focusing on quantum comparators—critical components in many quantum algorithms—this project provides a thorough analysis that helps designers choose the optimal circuit for their needs. The study includes an evaluation of the circuits based on metrics such as quantum cost, gate count, and fault tolerance.

## Features

- **Quantum Comparator Circuits:** A selection of quantum comparator circuits, implemented using various quantum gates such as Pauli gates, Hadamard, CNOT, and Toffoli gates.
- **Detailed Analysis:** Each comparator circuit is analyzed based on key metrics to help designers understand the trade-offs and advantages of each design.

## Results

The repository provides a detailed study of the quantum comparators, including a comparison based on metrics such as the number of quantum gates used, quantum cost, and efficiency. This analysis is designed to assist designers in selecting the most appropriate comparator for their specific requirements.

## Future Work

- Further exploration of additional quantum gates and their impact on comparator efficiency.
- Expansion of the analysis to include more complex quantum circuits and their potential applications.
- Continuous refinement of the metrics to ensure they remain relevant as quantum computing technology evolves.

## Acknowledgments

I would like to thank my advisors, Gloria Ortega López and Francisco José Orts Gómez, for their guidance throughout this project. Special thanks to the University of Almería and the Department of Computer Science for their support.
