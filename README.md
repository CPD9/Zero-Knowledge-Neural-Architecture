# Zero-Knowledge Neural Architecture (ZKNA)

## Overview
The **Zero-Knowledge Neural Architecture (ZKNA)** integrates **Zero-Knowledge Proofs (ZKPs)** and **Multi-Party Computation (MPC)** to create privacy-preserving machine learning models. This framework was specifically developed and tested for a scientific paper to showcase its ability to protect sensitive data during the training and inference phases while enabling model validation through Zero-Knowledge Proofs. ZKNA is particularly useful in scenarios where data privacy is critical, and regulatory compliance (e.g., GDPR, HIPAA) must be ensured.

## Scientific Paper
This project was designed as part of the research for the paper titled:
> **"Zero-Knowledge Neural Architecture for Privacy-Guaranteed Machine Learning"**  
> Authors: Mujahid M. Yaseen, Abdellatif O. Omar, and Dike C. Peter, Jr.

In the paper, ZKNA was evaluated for its effectiveness in creating a secure machine learning pipeline that ensures data privacy without sacrificing model accuracy.

## Features
- **Privacy Preservation**: Uses **homomorphic encryption** to secure data during processing and training, ensuring no sensitive data is exposed.
- **Multi-Party Computation (MPC)**: Enables **distributed training** and inference across multiple parties while keeping data encrypted and private.
- **Zero-Knowledge Proofs**: Verifies model results without revealing any sensitive data, leveraging ZKPs like **zk-SNARKs**.
- **Scalability**: Applicable in a wide range of industries, including **finance**, **healthcare**, and more, to meet stringent privacy and security requirements.

## Experimental Results
The results from the experiments conducted in the paper demonstrate the performance of the ZKNA framework on the **UCI Adult Dataset** for income classification. The following table summarizes key performance metrics:

| Model                   | Accuracy (%) | Training Latency (s) | Proof Size (MB) |
|-------------------------|--------------|----------------------|-----------------|
| **Standard Neural Network** | 82.8         | 120                  | N/A             |
| **Privacy-Preserving NN**   | 71.6         | 205                  | N/A             |
| **ZKNA**                    | 76.3         | 204                  | 1.2             |

### Key Insights:
- **ZKNA** achieves a balance between **accuracy** and **privacy**, with only a slight reduction in accuracy compared to the standard neural network due to encryption overhead.
- The **proof size** of 1.2 MB per instance showcases the scalability of zk-SNARKs in privacy-preserving machine learning workflows.

## Requirements
- Python 3.x
- Libraries: `tenseal`, `pytorch`, `scikit-learn`, `openvino`, `matplotlib`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ZKNA.git
