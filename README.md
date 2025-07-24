# Synthetic Linear Regression with NumPy, TensorFlow, and Matplotlib

This project demonstrates a complete workflow for:
- Generating a synthetic linear regression dataset using NumPy
- Training a simple neural network model to learn its mapping with TensorFlow/Keras
- Inspecting learned weights and bias
- Visualizing model outputs versus true targets using Matplotlib

---

## Overview

- **Features**: Two input variables (X₁, X₂), randomly sampled in [-10, 10]
- **Target generation rule**:  
y = 2 * X₁ - 3 * X₂ + 5 + noise
where `noise` is random in [-1, 1]
- **Model**: Single-layer (Dense) neural network
- **Goal**: Learn the original mapping and visualize prediction accuracy

---

## Project Workflow

### 1. Data Generation

A synthetic regression dataset is generated and saved as `data_set.npz`


---

### 2. Model Training

A minimal Keras model (single Dense layer) is trained on the generated data:

---

### 3. Inspecting Model Weights

After training, the learned weights and bias are extracted:

Compare these to the data’s original formula (`[2, -3]` and `5`).

---

### 4. Prediction and Comparison

Making and viewing predictions

---

### 5. Visualization

Plot the predicted outputs versus the true targets to gauge fit:
A well-trained model should produce points clustered along a diagonal.

---

## Usage Instructions

1. **Install dependencies** (NumPy, TensorFlow, Matplotlib):
    ```
    pip install numpy tensorflow matplotlib
    ```

2. **Copy the above code** into a single Python script (e.g., `main.py`), or split generation and training into `generate_dataset.py` and `train_model.py`.

3. **Run the script(s)** to generate the dataset, train the model, and visualize results.

---

## Project Structure
├── main.py # (or) generate_dataset.py + train_model.py
├── data_set.npz # Generated dataset

---

## Requirements

- Python 3.10
- NumPy 2.1.3
- TensorFlow 2.19.0
- Matplotlib
