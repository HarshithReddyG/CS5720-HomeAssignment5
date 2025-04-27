# Implementing a Basic GAN on MNIST Dataset

## Overview
This code demonstrates the implementation of a simple Generative Adversarial Network (GAN) using PyTorch. The primary focus is on:

- Defining a Generator and Discriminator architecture
- Training them alternately in an adversarial setup
- Generating handwritten digit images using the MNIST dataset

## Dataset
- **Dataset Used:** MNIST handwritten digits dataset.
- The dataset is loaded directly using PyTorch’s `torchvision.datasets`.
- No manual or external dataset required.

## Code Flow

### Data Loading
- Load MNIST dataset with normalization between [-1, 1].
- Set up a DataLoader for efficient mini-batch training.

### Defining Generator and Discriminator
- **Generator:**  
  Takes random noise and outputs 28x28 pixel images.
- **Discriminator:**  
  Takes an image and outputs a probability (real/fake).

### Training Loop
- **Step 1:** Train the Discriminator to distinguish real and fake images.
- **Step 2:** Train the Generator to fool the Discriminator.
- Losses of both Generator and Discriminator are recorded for plotting.

### Generating and Displaying Samples
- Generate and show fake images at:
  - **Epoch 0**
  - **Epoch 25**
  - **Epoch 50**

### Loss Plotting
- Plot the Generator and Discriminator losses over epochs.

## Installation & Requirements

### Running on Google Colab
- PyTorch and torchvision are pre-installed.
- No additional setup needed.
- If necessary, install using:
```python
!pip install torch torchvision
```

### Running on Local System
- Install packages:
```bash
pip install torch torchvision matplotlib
```

- Download MNIST automatically via `torchvision.datasets`.

## Running the Script
- If saved as a Python script (`ha5_3.py`):
```bash
python ha5_3.py
```
- Alternatively, run the notebook:
  - Open **HA5_3.ipynb** in Google Colab or Jupyter Notebook.
  - Run all cells sequentially.

## Output

### Image Samples
- Images generated at Epoch 0, 25, and 50 showing the GAN’s progress in creating digits.

### Loss Plots
- Line plots comparing Generator and Discriminator losses over training epochs.

Note: Open **HA5_3.ipynb** to view the generated outputs.

**Path:** Q3_GAN_Basic/HA5_3.ipynb

---

## Observations

- **GAN Adversarial Training:**
  - Generator improves over time in making realistic digits.
  - Discriminator tries to correctly distinguish real and fake digits.
  
- **Loss Behavior:**
  - Generator and Discriminator losses fluctuate due to adversarial competition.
  
- **Generated Images:**
  - Initially noisy, but get sharper and more digit-like after more epochs.

---

## Remarks
- Code is properly commented, explaining each step.
- The training is kept simple and efficient to run within reasonable time on Google Colab.
- For faster experiments, a smaller latent dimension and fewer epochs are used.

---

## Contact
- **Name:** Harshith Reddy Gundra
- **Student ID:** 700780724
- **Email:** hxg07240@ucmo.edu

**Code Path:** Q3_GAN_Basic/HA5_3.ipynb

