# Quantum Natural Gradient with Backtracking Line Search

This repository contains a Qiskit implementation of Quantum Natural Gradient with Backtracking Line Search implemented during the Cohort 6 of [QOSF mentorship program](https://qosf.org/qc_mentorship/).

## Table of Contents
* [Intoduction](#Intoduction)
* [Project Description](#Project-Description)
* [Code Description](#Code-Description)
* [Technologies](#Technologies)
* [How to Use](#How-to-Use)
* [Contributors](#Contributors)
* [References](#References)

# Intoduction

One of the challenges in machine learning is the computational expense of training machine learning models. A recent effort in the early adoption of quantum computers to train ML models has been actively explored by the scientific community. In particular, Prasanna Data has shown that the training of linear regression models on big datasets could be sped up 2.8 times when trained on adiabatic quantum computers. Matthias C. Caro et.al. researched the possibility of training ML models on gate-based quantum computers on a small dataset without the loss in quantity of the training. 

In this work, our team investigates the possibility of training ML models on near-term quantum devices. We explored the Quantum Natural Gradient with the backtracking line search as described in [1], and its implementation in IBM Qiskit as an extension of the NaturalGradient Class available in the Qiskit open-source framework.


# Project Description

The project was accomplished in several stages. First, we verify the results of the research paper Quantum Natural Gradient with Efficient Backtracking Line Search [1] using the IBM Qiskit framework. We have successfully reproduced the experiments on finding the electronic ground states of hydrogen (H), lithium hydride (LiH) molecules, and transverse field Ising model (TFI) using Qiskit. Secondly, we explored the possibility of extending the current implementation of the Qiskit NaturalGradient Class with the Backtracking Line search algorithm. The current implementation of the NaturalGradient search available in Qiskit relies on regularization procedures. That is, the algorithm balances between biases and overfitting to minimize the loss function efficiently. Finally, in our project, we introduce the NaturalGradient class with the backtracking line search based on the Armijo condition. 

# Code Description

The notebook [H_LiH_TIFModel](https://github.com/olgOk/Adaptive_QNG/blob/main/examples/H_LiH_TIFModel.ipynb) contains the reproduction of the experiments on H, LiH, and TFI in Qiskit environment.

The notebook [Tutorial_on_QFI_in_Qiskit.ipynb](https://github.com/olgOk/Adaptive_QNG/blob/main/examples/Tutorial_on_QFI_in_Qiskit.ipynb) contains the example of Quantum Fisher Information (QFI) calculation in Qiskit. The QFI has a meaning of sensitivity to change the parameters of a parametrized circuit since the QFI is the second order derivative of a circuit by its parameters and is an approximation of the parametric surface.

The notebook [Backtracking-Line_Search](https://github.com/olgOk/Adaptive_QNG/blob/main/code/Backtracking-Line_Search.ipynb) contains a simple implementation of the Backtracking Line search based on Armijo's rule.

# Technologies

* Python3
* Qiskit
* Qiskit QML

# How to Use

### Local Environment.
Git clone repository and open files Jupyter Notebook. For a better experience, use a virtual environment settings. Each files contains the instructions for the required frameworks installation.

### Google Colab. 
Open files in Google Colab environment.

### IBM Quantum Lab. 
Upload to IBM Quantum Lab computing services to execute code in notebooks. 


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