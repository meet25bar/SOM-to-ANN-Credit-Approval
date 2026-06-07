# SOM-to-ANN-Credit-Approval


A hybrid machine learning project that combines Self-Organizing Maps (SOM) and Artificial Neural Networks (ANN) to identify high-risk applicants and predict credit card approval outcomes. The model leverages unsupervised learning for anomaly detection and supervised learning for accurate classification.

---

## 📌 Overview

Financial institutions receive thousands of credit card applications every day. Identifying risky applicants while ensuring accurate approval decisions is a critical challenge.

This project implements a two-stage machine learning pipeline:

1. **Self-Organizing Maps (SOM)** detect potential anomalies and high-risk applicants.
2. **Artificial Neural Networks (ANN)** use the information discovered by the SOM to predict credit card approval outcomes.

This hybrid approach combines the strengths of both unsupervised and supervised learning techniques.

---

## 🎯 Objectives

- Detect unusual or potentially risky applicants using SOM.
- Build an ANN classifier for credit approval prediction.
- Demonstrate the integration of unsupervised and supervised learning.
- Improve decision-making in credit risk assessment.

---

## 📂 Dataset

The project uses the **Credit Card Applications Dataset**, which contains applicant information such as:

- Age
- Income-related attributes
- Employment information
- Credit history indicators
- Other financial features

**Target Variable:**
- `Class = 1` → Approved
- `Class = 0` → Rejected

---

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- MiniSom
- TensorFlow / Keras

---

## 🔍 Project Workflow

### 1. Data Preprocessing
- Load dataset
- Handle missing values
- Feature scaling using MinMaxScaler
- Prepare input features and labels

### 2. Self-Organizing Map (SOM)
- Train SOM on customer application data
- Visualize distance map
- Identify anomalous/high-risk applicants

### 3. Fraud Risk Identification
- Extract suspicious customers from SOM clusters
- Create a fraud-risk indicator

### 4. Artificial Neural Network (ANN)
- Build ANN using Keras
- Train model using customer features
- Predict approval probability for each applicant

### 5. Evaluation
- Analyze prediction probabilities
- Rank applicants based on risk level
- Compare results with actual outcomes

---

## 📊 Model Architecture

### Self-Organizing Map
- Input Layer: Customer Features
- SOM Grid: 10 × 10
- Learning Rate: 0.5
- Sigma: 1.0

### Artificial Neural Network
- Input Layer
- Hidden Layer (ReLU Activation)
- Output Layer (Sigmoid Activation)

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/SOM-to-ANN-Credit-Approval.git
cd SOM-to-ANN-Credit-Approval
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the notebook:

```bash
jupyter notebook som.ipynb
```

Or execute the Python script:

```bash
python main.py
```

---

## 📈 Results

- Successfully identified anomalous customer profiles using SOM.
- Built an ANN classifier to estimate approval likelihood.
- Demonstrated how unsupervised learning can enhance supervised prediction performance.

---

## 📁 Repository Structure

```text
SOM-to-ANN-Credit-Approval/
│
├── data/
│   └── Credit_Card_Applications.csv
│
├── notebooks/
│   └── som.ipynb
│
├── images/
│   ├── som_distance_map.png
│   └── architecture.png
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🔮 Future Improvements

- Hyperparameter tuning
- Cross-validation
- Advanced anomaly detection techniques
- Deployment using Flask/FastAPI
- Interactive dashboard for risk analysis

---

## 👨‍💻 Author

**Met Barot**

B.Tech Computer Science Student  
Interested in Machine Learning, Deep Learning, and AI Applications in Finance.

---

## ⭐ Acknowledgements

- UCI Machine Learning Repository
- MiniSom Library
- TensorFlow/Keras
- Scikit-learn Community

If you found this project useful, consider giving it a ⭐ on GitHub!
