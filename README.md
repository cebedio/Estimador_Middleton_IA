This repository contains the complete development flow of an AI-based estimator for Middleton Class-A noise parameters, including data generation, model training and validation, and hardware implementation as an FPGA IP core.

The project is intended for embedded and real-time signal-processing applications, where non-Gaussian impulsive noise modeling is required and computational resources are constrained.

## Repository Structure
├── Generar_datos_middleton.ipynb
├── Entrenamiento_e_implementación_estimador_Middleton.ipynb
├── vhdl/
├── verilog/
└── README.md.

## Main Components:

1. Data Generation
 - Generar_datos_middleton.ipynb
 - Generation of synthetic datasets following the Middleton Class-A noise model.
 - Configurable parameters (e.g., impulsive index, Gaussian variance, mixture coefficients).
 - Output datasets used for training and validation of the AI model.

2. AI Model Training and Validation
   - Entrenamiento_e_implementación_estimador_Middleton.ipynb
   - Training of a neural-network-based estimator for Middleton noise parameters.
   - Model validation and performance evaluation.
   - Preparation of the trained model for hardware implementation.

3. FPGA Hardware Implementation
   - vhdl/
   - verilog/
   - HDL descriptions (VHDL and Verilog) corresponding to the synthesized FPGA IP core.

The IP core acts as a hardware accelerator for real-time noise parameter estimation.
Suitable for integration in embedded DSP systems and SoC designs.

## Design Flow Overview:
 - Synthetic data generation using the Middleton Class-A noise model
 - AI model training and validation in Python
 - Model export and hardware mapping
 - HDL generation (VHDL / Verilog)
 - FPGA synthesis and integration as an IP core

## Requirements
 - Python 3.x
 - NumPy, SciPy
 - Machine Learning framework used in the notebooks (e.g., TensorFlow / Keras or equivalent)
 - FPGA toolchain for synthesis (vendor-specific, not included)

## Intended Applications
 - Embedded communication systems affected by impulsive noise
 - Submarine and underwater acoustic communications
 - Power-line communications (PLC)
 - Real-time digital signal processing on FPGA

## Notes:
The notebooks are intended as reference implementations and may require adaptation depending on the target FPGA platform.
HDL files correspond to the final synthesized architecture used in the proposed system.

## License: This project is provided for research and academic purposes. Please contact the authors for usage beyond these terms.
