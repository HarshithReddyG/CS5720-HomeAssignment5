# Data Poisoning Simulation on Sentiment Classifier (Final Version)

## Overview
This code simulates a basic data poisoning attack on a sentiment classifier using an expanded small dataset. The main focus is:

- Training a baseline sentiment classifier on movie reviews.
- Poisoning the training data by flipping labels for sentences mentioning "UC Berkeley".
- Comparing model performance before and after poisoning.

## Dataset
- Manually created dataset with 20 sentences (positive and negative sentiment).
- Includes multiple sentences mentioning "UC Berkeley".
- Balanced distribution of positive and negative labels.

## Code Flow

### Data Preparation
- Sentences and labels are organized into a pandas DataFrame.
- Sentences about "UC Berkeley" are included for poisoning.

### Preprocessing
- Sentences are vectorized using `CountVectorizer`.
- Train-test split is performed using stratified sampling to maintain class balance.

### Training the Basic Classifier (Before Poisoning)
- A Logistic Regression model is trained on the clean data.
- Accuracy and confusion matrix are computed.

### Data Poisoning
- Sentences containing "UC Berkeley" have their sentiment labels flipped.

### Training the Classifier After Poisoning
- A new Logistic Regression model is trained on the poisoned data.
- Accuracy and confusion matrix are recomputed.

### Visualization
- Bar plot comparing accuracy before and after poisoning.
- Heatmaps of confusion matrices before and after poisoning.

## Installation & Requirements

### Running on Google Colab
- Required libraries are usually pre-installed.

If needed, install manually:
```python
!pip install scikit-learn pandas matplotlib seaborn
```

### Running on Local System
```bash
pip install scikit-learn pandas matplotlib seaborn
```

## Running the Script
- If saved as a Python file (`ha5_4.py`):
```bash
python ha5_4.py
```
- Alternatively, open and run the provided Jupyter Notebook **HA5_4.ipynb** in Google Colab or Jupyter Notebook.

## Output

### Graphs and Visualizations
- Bar chart comparing model accuracy before and after poisoning.
- Heatmaps of confusion matrices showing classification results.

### Observations
- Model accuracy drops after data poisoning.
- Confusion matrix shows an increase in misclassifications.
- Flipping labels for "UC Berkeley" sentences causes confusion in the model, demonstrating the effectiveness of the data poisoning attack.

Note: Open **HA5_4.ipynb** to view full outputs.

**Path:** Q4_Data_Poisoning/HA5_4.ipynb

---

## Remarks
- Code is properly commented.
- Expanded dataset ensures more stable training and evaluation.
- Demonstrates a clear, understandable simulation of a real-world data poisoning attack.

---

## Contact
- **Name:** Harshith Reddy Gundra
- **Student ID:** 700780724
- **Email:** hxg07240@ucmo.edu

**Code Path:** Q4_Data_Poisoning/HA5_4.ipynb

