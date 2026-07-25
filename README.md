# 🩺 Diabetes Prediction using Artificial Neural Network (ANN)

A Deep Learning project that predicts whether a patient is likely to have diabetes using an Artificial Neural Network (ANN) built with TensorFlow and Keras.

---

## 📌 Project Overview

This project uses the **Pima Indians Diabetes Dataset** to build a binary classification model capable of predicting whether a patient has diabetes based on several medical attributes.

The project covers the complete Deep Learning workflow, including:

- Data Loading
- Data Preprocessing
- Train-Test Split
- Feature Scaling
- Building an Artificial Neural Network (ANN)
- Model Training
- Model Evaluation
- Performance Visualization
- Prediction on Unseen Data

---

## 📂 Dataset

**Dataset:** Pima Indians Diabetes Dataset

Features:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

Target:

- Outcome
  - 0 → No Diabetes
  - 1 → Diabetes

Number of Samples:

- 768

---

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 📚 Workflow

### 1. Data Loading

- Loaded the dataset using Pandas.

### 2. Data Preprocessing

- Separated Features (X) and Target (y).
- Split the dataset into Training and Testing sets.
- Applied StandardScaler for feature normalization.

### 3. Model Architecture

The ANN consists of:

- Input Layer (8 Features)
- Hidden Layer
  - 16 Neurons
  - ReLU Activation
- Hidden Layer
  - 8 Neurons
  - ReLU Activation
- Output Layer
  - 1 Neuron
  - Sigmoid Activation

---

## ⚙ Model Compilation

Optimizer:

- Adam

Loss Function:

- Binary Crossentropy

Evaluation Metric:

- Accuracy

---

## 🚀 Model Training

The model was trained using:

- Epochs: 100
- Batch Size: 32
- Validation Split: 20%
- EarlyStopping Callback

EarlyStopping was used to:

- Monitor Validation Loss
- Prevent Overfitting
- Restore the Best Model Weights

---

## 📈 Model Evaluation

The model was evaluated using:

- Test Accuracy
- Test Loss
- Confusion Matrix
- Classification Report
- ROC Curve
- ROC-AUC Score

---

## 📊 Results

### Test Accuracy

```text
75.32%
```

### ROC-AUC Score

```text
0.813
```

### Confusion Matrix

```text
[[79 20]
 [18 37]]
```

### Classification Report

```text
              precision    recall  f1-score   support

           0       0.81      0.80      0.81        99
           1       0.65      0.67      0.66        55

    accuracy                           0.75       154
   macro avg       0.73      0.74      0.73       154
weighted avg       0.76      0.75      0.75       154
```

---

## 📉 Training Performance

The following graphs were generated during training:

- Training Loss vs Validation Loss
- Training Accuracy vs Validation Accuracy
- ROC Curve

These visualizations help analyze:

- Model Learning
- Overfitting
- Generalization Performance
- Classification Ability

---

## 📁 Project Structure

```text
diabetes-prediction-deep-learning/
│
├── data/
│   └── diabetes.csv
│
├── notebooks/
│   └── diabetes_prediction_ann.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🎯 Key Learning Outcomes

Through this project, I learned:

- Data preprocessing for Deep Learning
- Feature scaling using StandardScaler
- Building ANN models with TensorFlow/Keras
- Understanding Dense layers
- ReLU and Sigmoid activation functions
- Binary Crossentropy Loss
- Adam Optimizer
- EarlyStopping
- Model Evaluation
- Confusion Matrix
- Precision, Recall and F1-score
- ROC Curve and ROC-AUC

---

## 🔮 Future Improvements

Possible enhancements include:

- Handling missing or invalid values using SimpleImputer
- Building a preprocessing Pipeline
- Hyperparameter tuning
- Saving the trained model
- Deploying the model using Streamlit
- Dockerizing the application
- Cloud deployment

---

## 👨‍💻 Author

**Abhihail Jacob**

AI/ML Engineer passionate about Machine Learning, Deep Learning, and building practical AI solutions.

---

## ⭐ Acknowledgement

This project was built as part of my Deep Learning learning journey to gain hands-on experience in designing, training, evaluating, and interpreting Artificial Neural Networks using TensorFlow and Keras.