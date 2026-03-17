# Iris Species Classification

A deep learning project implementing multi-class classification to predict iris flower species using a feedforward neural network with Keras and TensorFlow.

## Overview

This project demonstrates a complete machine learning workflow including data preprocessing, model architecture design, training, and evaluation. The model predicts iris species (Setosa, Versicolor, Virginica) based on four morphological features using a neural network with 100% test accuracy.

## Dataset

The Iris dataset contains 150 flower samples with 4 continuous features per sample:
- Sepal Length (cm)
- Sepal Width (cm)
- Petal Length (cm)
- Petal Width (cm)

Target: 3 iris species (categorical)

## Project Structure

```
iris-classifier/
├── iris-species.ipynb          # Main implementation notebook
├── README.md                   # Project documentation
├── requirements.txt            # Python dependencies
└── .gitignore                  # Git ignore file
```

## Methodology

### 1. Data Preprocessing
- Dataset normalization using Min-Max scaling (0-1 range)
- One-hot encoding of categorical target variable
- Train-test split: 70% training, 30% testing

### 2. Model Architecture
```
Input Layer (4 features)
    ↓
Dense Layer (64 neurons, ReLU activation)
    ↓
Dense Layer (64 neurons, ReLU activation)
    ↓
Output Layer (3 neurons, Softmax activation)
```

### 3. Training Configuration
- **Optimizer**: Adam (adaptive learning rate)
- **Loss Function**: Categorical Crossentropy
- **Metrics**: Accuracy
- **Epochs**: 100
- **Batch Size**: Default (32)

## Results

| Metric | Value |
|--------|-------|
| Test Accuracy | 100.0% |
| Test Loss | 0.0733 |
| Training Samples | 105 |
| Testing Samples | 45 |

## Installation

1. Clone the repository:
```bash
git clone git@github.com:Devaaldo/iris-species-classification.git
cd iris-classifier
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/Scripts/activate  # On Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

Run the Jupyter notebook:
```bash
jupyter notebook iris-species.ipynb
```

The notebook will execute all stages: data loading, preprocessing, model training, and evaluation.

## Key Features

- Complete data science workflow from raw data to predictions
- Well-documented code with professional comments
- High-performance model with 100% test accuracy
- Reproducible results with seed-based splitting
- Efficient preprocessing pipeline

## Technologies

- **Python 3.8+**
- **TensorFlow/Keras** - Deep learning framework
- **Pandas** - Data manipulation
- **NumPy** - Numerical computing
- **Scikit-learn** - Preprocessing and model evaluation

## Performance Notes

The model achieves perfect accuracy on the test set, indicating the dataset characteristics and model complexity are well-matched. The Iris dataset is a small, well-separated classification problem suitable for demonstrating neural network fundamentals.

## License

This project is open source and available under the MIT License for educational and research purposes.
