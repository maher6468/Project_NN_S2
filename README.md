# Neural Networks Course Project  
## Student Performance Classification using Multilayer Perceptron (MLP)

## Project Overview
This project applies a Multilayer Perceptron (MLP) neural network to classify student academic performance based on several educational and behavioral features. The goal is to predict the final student grade using machine learning and deep learning techniques. The project was implemented using PyTorch and follows the requirements of the Neural Networks course project.

---

## Dataset
The dataset contains information about students, including:

- Study hours
- Attendance percentage
- Assignment scores
- Midterm scores
- Participation scores
- Sleep hours
- Parent education level
- Internet access
- Extracurricular activities

### Target Variable
`grade`

The grades were classified into multiple classes:
- A
- B
- C
- D
- F

---

## Data Preprocessing
The following preprocessing steps were applied:

- Removing unnecessary columns (`student_id`)
- Handling categorical variables using encoding
- Feature scaling using `StandardScaler`
- Splitting the dataset into training and testing sets

---

## Model Architecture
A Multilayer Perceptron (MLP) was implemented using PyTorch.

Architecture:
Input Layer → Hidden Layer (128) → Hidden Layer (64) → Output Layer (5)

### Activation Functions
- ReLU
- Tanh

### Loss Function
- CrossEntropyLoss

### Optimizer
- Adam

---

## Experiments

| Experiment | Configuration | Test Accuracy |
|---|---|---|
| Experiment 1 | ReLU Activation | 97.25% |
| Experiment 2 | Tanh Activation | 98.15% |
| Experiment 3 | ReLU + Dropout | 97.30% |

---

## Results
- The Tanh activation function achieved the highest accuracy.
- Dropout helped reduce overfitting but did not significantly improve the final accuracy.
- The model achieved excellent classification performance overall.

### Best Accuracy
98.15%

---

## Visualizations
The following visualizations were included:

- Training vs Validation Loss Curves
- Training vs Validation Accuracy Curves
- Confusion Matrix

---

## Technologies Used
- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## How to Run

### Clone the repository
```bash
git clone <your-repository-link>
