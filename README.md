# Home Assignment 5 - Generative AI, Fairness, and Security

## Overview
This repository contains the solutions for Home Assignment 5, focusing on Generative Adversarial Networks (GANs), data poisoning attacks, legal/ethical implications of generative AI, and bias/fairness audit tools.

The assignment is divided into two major coding tasks and an answer document:

- **Q3_GAN_Basic/** — Basic GAN implementation on MNIST dataset.
- **Q4_Data_Poisoning/** — Simulation of a data poisoning attack on a sentiment classifier.
- **answers.pdf** — Answers to theoretical questions (1, 2, 5, and 6).

---

## Repository Structure

```
HomeAssignment5/
|
|-- Q3_GAN_Basic/
|     |-- HA5_3.ipynb          # Basic GAN Implementation on MNIST
|     |-- README.md            # ReadMe for Q3_GAN_Basic
|
|-- Q4_Data_Poisoning/
|     |-- HA5_4.ipynb    # Data Poisoning Simulation
|     |-- README.md            # ReadMe for Q4_Data_Poisoning
|
|-- answers.pdf                # Written answers for Q1, Q2, Q5, and Q6
|
|-- README.md                  # Main repository ReadMe (this file)
```

---

## Project Details

### Q3_GAN_Basic
- Implemented a basic Generative Adversarial Network (GAN) using PyTorch.
- Generated handwritten digits from the MNIST dataset.
- Plotted generated images at epochs 0, 25, and 50.
- Compared Generator and Discriminator losses over training.

**Path:** Q3_GAN_Basic/HA5_3.ipynb

### Q4_Data_Poisoning
- Built a small sentiment analysis classifier using Logistic Regression.
- Simulated a targeted data poisoning attack by flipping labels for specific entity mentions ("UC Berkeley").
- Analyzed and compared model accuracy and confusion matrices before and after poisoning.

**Path:** Q4_Data_Poisoning/HA5_4.ipynb

### answers.pdf
- Written responses to:
  - Q1: GAN Architecture and Adversarial Process
  - Q2: Ethics and AI Harm
  - Q5: Legal and Ethical Implications of GenAI
  - Q6: Bias & Fairness Tools (Aequitas False Negative Rate Parity)

**Path:** answers.pdf

---

## Requirements
- Python 3.8+
- Libraries: torch, torchvision, scikit-learn, pandas, matplotlib, seaborn
- Recommended environment: Google Colab

Installation (if needed locally):
```bash
pip install torch torchvision scikit-learn pandas matplotlib seaborn
```

---

## Contact
- **Name:** Harshith Reddy Gundra
- **Student ID:** 700780724
- **Email:** hxg07240@ucmo.edu

---

## Notes
- All code files are commented for clarity.
- Each subfolder includes its own specific README.
- answers.pdf contains concise, direct answers based on lecture material and instructions.

---

Thank you for reviewing Home Assignment 5!

