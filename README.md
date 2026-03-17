# Iris Species Classification

A deep learning project for classifying iris flower species using a neural network trained on the classic Iris dataset.

## Overview

This project implements a multi-class classification model to predict iris species based on four morphological features: sepal length, sepal width, petal length, and petal width. The model uses a sequential neural network built with Keras to classify flowers into three species: Iris setosa, Iris versicolor, and Iris virginica.

## Dataset

The Iris dataset contains 150 samples with 4 features per flower:
- Sepal Length (cm)
- Sepal Width (cm)
- Petal Length (cm)
- Petal Width (cm)

Target classes: 3 iris species

## Project Structure

- `iris-species.ipynb` - Main Jupyter notebook containing data preprocessing, model training, and evaluation

## Methodology

1. **Data Collection**: Loaded Iris dataset from external source
2. **Preprocessing**:
   - Removed ID column
   - One-hot encoded categorical target variable
   - Applied Min-Max normalization to features (0-1 range)
3. **Model Architecture**:
   - Input layer: 4 features
   - Hidden layer 1: 64 neurons with ReLU activation
   - Hidden layer 2: 64 neurons with ReLU activation
   - Output layer: 3 neurons with Softmax activation
4. **Training**:
   - Optimizer: Adam
   - Loss function: Categorical Crossentropy
   - Epochs: 100
   - Train-test split: 70-30

## Results

- Test Accuracy: 100%
- Test Loss: 0.073

## Requirements

- Python 3.8+
- pandas
- scikit-learn
- keras
- numpy

## Usage

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Run the notebook:
```bash
jupyter notebook iris-species.ipynb
```

## License

This project is open source and available for educational purposes.
