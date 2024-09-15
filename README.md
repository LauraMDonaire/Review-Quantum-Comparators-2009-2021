# Review of Quantum Comparators

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

#### 2. Half - Comparator

A **medium comparator** determines whether one value A is greater than or equal to another value B (i.e., A ≥ B). This type of comparator goes beyond mere equality and is useful in scenarios where a more nuanced comparison is required.

#### 3. Full Comparator

A **full comparator** performs a more comprehensive comparison by checking whether A is greater than B, equal to B, or less than B (i.e., A > B, A = B, or A < B). This type of comparator provides a complete comparison of the two values and is used when detailed relational information is needed.

In this work, we focus on **half-comparators**, but some **full comparators** will also be studied, even though they are not included in Table 1.

## Motivation

The motivation behind this project is to address the growing need for efficient quantum circuits as quantum computing continues to advance. By focusing on quantum comparators—critical components in many quantum algorithms—this project provides a thorough analysis that helps designers choose the optimal circuit for their needs. The study includes an evaluation of the circuits based on metrics such as quantum cost, gate count, and fault tolerance.

## Features

- **Quantum Comparator Circuits:** A selection of quantum comparator circuits, implemented using various quantum gates such as Pauli gates, Hadamard, CNOT, and Toffoli gates.
- **Detailed Analysis:** Each comparator circuit is analyzed based on key metrics to help designers understand the trade-offs and advantages of each design.

## Results

The repository provides a detailed study of the quantum comparators, including a comparison based on metrics such as the number of quantum gates used, quantum cost, and efficiency. This analysis is designed to assist designers in selecting the most appropriate comparator for their specific requirements. 

### Overview of Circuit Metrics

Tables 1 and 2 show the metrics of the circuits studied in this work. For clarity, these studies have worked with numbers of a specific size. For example, the circuit by Orts et al. shown [here](./Half-Comparators/Orts%20et%20al.%202021/Orts's%20Quantum%20Half%20Comparator(n=8).pdf) is adapted to work with 8-digit numbers. However, it is clear that these circuits can be adapted to any size $n$. Since comparing circuits that work with different sizes is highly inefficient, Tables 1 and 2 do not show specific values. Instead, the equations used to calculate each metric in the general case are shown, i.e., for a generic number size $n$ digits (for each number compared, that is, to compare two numbers of $n$ digits).

### Table 1: General Equations for Cost and Delay of the Reviewed Comparators

| Comparator | Cost | Delay |
|------------|------|-------|
| Thapliyal et al. [[1]](#1) | $13.5n + 27\log(2^n) + 1$ | $9n + 18\log(2^n) + 1$|
| Xia et al. (2018) [[2]](#2) | $36n$ | $27n + 6$ |
| Xia et al. (2019) [[3]](#3) | $18n - 12$ | $14n - 7$ |
| Li et al. (2020) [[4]](#4) | $12n - 8$ | $10n - 6$ |
| Orts et al. (a) [[5]](#5) | $22n - 10$ | $18n - 8$ |
| Orts et al. (b) [[5]](#5) | $\approx 32n + 46\log(n)$ | $\log(n)$ |

### Table 2: General Equations for T-count, T-depth, and Auxiliary Bits of the Reviewed Comparators

| Comparator              | T-count                                | T-depth                               | Auxiliary                           |
|-------------------------|----------------------------------------|---------------------------------------|-------------------------------------|
| Thapliyal et al. [[1]](#1)    | $21n + 42\log(2^n) + 1$               | $8n + 16\log(2^n) + 1$               | $n + 2\log(2^n) + 1$               |
| Xia et al. (2018) [[2]](#2)   | $28n$                                 | $12n$                                 | $3$                                  |
| Xia et al. (2019) [[3]](#3)   | $18n - 12$                            | $6n - 3$                              | $2n$                                 |
| Li et al. (2020) [[4]](#4)    | $14n - 8$                             | $4n - 2$                              | $2n$                                 |
| Orts et al. (a) [[5]](#5)     | $4n$                                  | $2n$                                  | $1$                                  |
| Orts et al. (b) [[5]](#5)     | $12n - 8W(n) - 4\log(n)$              | $\log(n)$                             | $4n - 2W(n) - 2\log(n)$            |

Table 1 compares the quantum cost and delay of various half-comparators. The half-comparators proposed by Al-Rabadi, Thapliyal, and Orts et al. (b) exhibit logarithmic cost and delay, while the others show linear behavior.

- **Quantum Cost**: Li et al. offer the most efficient half-comparator with a quantum cost of $12n - 8$. In contrast, Xia et al. (2018) have the highest cost at $36n$, making it three times less efficient than Li et al.
  
- **Quantum Delay**: Orts et al. (b) propose the best half-comparator with a logarithmic delay of $\log(n)$. The least efficient in terms of delay is Xia et al. (2018) with $27n + 6$.

Table 2 provides a comparison in terms of T-count, T-depth, and auxiliary inputs:

- **T-count**: Orts et al. (a) achieves the lowest T-count with $4n$, while Thapliyal et al. have the highest at $21n + 42\log(2n) + 1$, making it eight times larger.
  
- **T-depth**: Al-Rabadi, Thapliyal, and Orts offer logarithmic T-depth, with Orts et al. being the best at $\log(n)$, while Thapliyal et al. have the highest T-depth.
  
- **Auxiliary Inputs**: Li et al. present the most efficient design with only one auxiliary input. In contrast, Al-Rabadi et al. require the most at $3n$.

## Future Work

- Further exploration of additional quantum gates and their impact on comparator efficiency.
- Expansion of the analysis to include more complex quantum circuits and their potential applications.
- Continuous refinement of the metrics to ensure they remain relevant as quantum computing technology evolves.

## References 
- <a name="1">[1]</a> H. Thapliyal, N. Ranganathan, and R. Ferreira, “Design of a comparator tree based on reversible logic,” 2010 10th IEEE Conference on Nanotechnology, pp. 1113–1116, 2010. [DOI: 10.1109/NANO.2010.5697872](https://doi.org/10.1109/NANO.2010.5697872)
- <a name="2">[2]</a> H. Xia, H.-S. Li, and H. Zhang, “An efficient design of reversible multi-bit quantum comparator via only a single ancillary bit,” *International Journal of Theoretical Physics*, vol. 57 (12), pp. 3727–3744, 2018. [DOI: 10.1007/s10773-018-3886-0](https://doi.org/10.1007/s10773-018-3886-0)
- <a name="3">[3]</a> H. Xia, H.-S. Li, H. Zhang, Y. Liang, and J. Xin, “Novel multi-bit quantum comparators and their application in image binarization,” *Quantum Information Processing*, vol. 18 (7), p. 229, 2019. [DOI: 10.1007/s11128-019-2334-2](https://doi.org/10.1007/s11128-019-2334-2)
- <a name="4">[4]</a> H.-S. Li, P. Fan, H. Xia, H. Peng, and G. Long, “Efficient quantum arithmetic operation circuits for quantum image processing,” *Science China Physics, Mechanics & Astronomy*, vol. 63, pp. 1–13, 2020. [DOI: 10.1007/s11433-020-1582-8](https://doi.org/10.1007/s11433-020-1582-8)
- <a name="5">[5]</a> F. Orts, G. Ortega, A.C. Cucura, E. Filatovas, and E.M. Garzón, “Optimal fault-tolerant quantum comparators for image binarization,” *The Journal of Supercomputing*, vol. 77, 2021. [DOI: 10.1007/s11227-020-03576-5](https://doi.org/10.1007/s11227-020-03576-5)
  
## Acknowledgments

I would like to thank my advisors, Gloria Ortega López and Francisco José Orts Gómez, for their guidance throughout this project. Special thanks to the University of Almería and the Department of Computer Science for their support.

## How to Cite

If you find this work useful and wish to cite it, please use the following reference:

Donaire, L. M., Ortega, G., Garzón, E. M., & Orts, F. (2024). Lowering the cost of quantum comparator circuits. Journal of Supercomputing, 80, 13900–13917. https://doi.org/10.1007/s11227-024-05959-4

## Contact

For more information, suggestions, or collaboration, you can contact:

- **Laura M. Donaire** (TIC-146 Supercomputación-Algoritmos [SAL], University of Almería): [laura.donaire@ual.es](mailto:laura.donaire@ual.es)
