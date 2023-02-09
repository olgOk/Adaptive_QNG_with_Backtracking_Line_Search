# Quantum Natural Gradient with Backtracking Line Search

This repository contains a Qiskit implementation of Quantum Natural Gradient with Backtracking Line Search.

## Table of Contents
* [Intoduction](#Intoduction)
* [Project Description](#Project-Description)
* [Technologies](#Technologies)
* [Code](#Code)
* [References](#References)
* [Contributors](#Contributors)

# Intoduction

One of the challenges in machine learning is the computational expense of training machine learning models. A recent effort in the early adoption of quantum computers to train ML models has been actively explored by the scientific community. In particular, Prasanna Data has shown that the training of linear regression models on big datasets could be sped up 2.8 times when trained on adiabatic quantum computers. Matthias C. Caro et.al. researched the possibility of training ML models on gate-based quantum computers on a small dataset without the loss in quantity of the training. 

In this work, our team investigates the possibility of training ML models on near-term quantum devices. We explored the Quantum Natural Gradient with the backtracking line search as described in [1], and its implementation in IBM Qiskit as an extension of the NaturalGradient Class available in the Qiskit open-source framework.


# Project Description

The project was accomplished in several stages. First, we verify the results of the research paper Quantum Natural Gradient with Efficient Backtracking Line Search using the IBM Qiskit framework. [Elaborate more] Secondly, we explored the possibility of extending the current implementation of the Natural Gradient with the Backtracking Line search. [Elaborate more]. Finally, we started the implementation of the backtracking line search [Elaborate more].

# Technologies
* Python3
* Qiskit
* Qiskit QML

# Code

# Contributors
Mentor: [Dr. Vesselin G. Gueorguiev](https://github.com/VGGatGitHub)

Team:

1. [Pritom Mozumdar](https://github.com/pmozumdar)
2. [Elias Lehman](https://github.com/eliaslehman)
3. [Olga Okrut](https://github.com/olgOk)

# References

1. [Touheed Anwar Atif, Uchenna Chukwu, Jesse Berwald, Raouf Dridi. Quantum Natural Gradient with Efficient Backtracking Line Search. Nov, 2022.](https://doi.org/10.48550/arXiv.2211.00615)
2. [Maria Schuld, Ville Bergholm, Christian Gogolin, Josh Izaac, Nathan Killoran. Evaluating analytic gradients on quantum hardware. November 2018. Phys. Rev. A 99, 032331 (2019).](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.99.032331)
3. [Real Amplitudes. Qiskit Tutotrial. IBM Q. ](https://qiskit.org/documentation/stubs/qiskit.circuit.library.RealAmplitudes.html)
4. [Qiskit Gradient Framework. Qiskit Tutorial. IBM Q.](https://qiskit.org/documentation/tutorials/operators/02_gradients_framework.html)