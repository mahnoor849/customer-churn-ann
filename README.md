# Customer Churn Prediction Using ANN

A machine-learning project that uses an Artificial Neural Network (ANN) to predict whether a bank customer is likely to churn.

## Overview

The project uses the commonly used **Churn Modelling** dataset with customer attributes such as credit score, geography, gender, age, tenure, balance, number of products, activity status, and estimated salary.

The target variable is `Exited`:

- `1` — customer left
- `0` — customer stayed

## Workflow

1. Load the churn dataset
2. Select predictive features and target
3. Encode categorical variables
4. Split data into training and test sets
5. Standardize features
6. Build and train a TensorFlow/Keras ANN
7. Evaluate predictions with accuracy and a confusion matrix
8. Run an example prediction for a single customer

## Model Architecture

- Dense layer: 6 neurons, ReLU
- Dense layer: 6 neurons, ReLU
- Output layer: 1 neuron, Sigmoid
- Optimizer: Adam
- Loss: Binary Crossentropy
- Metric: Accuracy
- Epochs: 100
- Batch size: 32

## Reported Results

The accompanying academic report records approximately:

- Training accuracy: **86.6%**
- Test accuracy: **86%**

Exact results may vary slightly between runs because neural-network training can be stochastic.

## Tech Stack

- Python
- TensorFlow / Keras
- Pandas
- NumPy
- scikit-learn
- Matplotlib
- Seaborn
- Jupyter / Google Colab

## Dataset

The notebook expects:

```text
Churn_Modelling.csv
```

The dataset itself is not bundled in this public repository. Add your own legally obtained copy to the project directory before running.

## Run

Install dependencies:

```bash
pip install -r requirements.txt
```

Then open:

```text
customer_churn_ann.ipynb
```

If running outside Google Colab, you can skip the initial `files.upload()` cell and place `Churn_Modelling.csv` directly in the project folder.

## Academic Scope

This is an educational machine-learning project and not a production banking model. It should not be used for real customer decisions without appropriate data governance, validation, fairness testing, security controls, and monitoring.

## Author

Mahnoor Yasin  
BS Computer Science
