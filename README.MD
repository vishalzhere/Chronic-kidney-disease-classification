🧬 Chronic Kidney Disease Detection Using Machine Learning
🩺 Project Synopsis

Chronic Kidney Disease (CKD) is a progressive medical condition that often remains undiagnosed until reaching advanced stages. This project presents a machine learning–driven diagnostic framework designed to predict the presence of CKD using routinely collected clinical and laboratory parameters.

The objective of this task is to demonstrate how data-driven models can support early-stage medical decision-making by identifying high-risk patients with high accuracy and reliability.

📊 Dataset Overview

Dataset: Chronic Kidney Disease Dataset

Total Records: 400 patient instances

Target Classes:

ckd – Chronic Kidney Disease

notckd – No Chronic Kidney Disease

Feature Composition:

24 clinical and laboratory attributes

Mixed data types (numerical + categorical)

Missing Values: Present and denoted by "?"

The dataset closely resembles real-world clinical data, making preprocessing and feature handling a crucial component of this task.

🧠 Methodology & Workflow
🔹 1. Data Preparation & Cleaning

Converted raw dataset into a structured CSV format

Handled missing values using appropriate statistical techniques

Encoded categorical variables into numerical representations

Ensured consistent data types across all features

Applied feature scaling using StandardScaler to improve model convergence

🔹 2. Exploratory Data Analysis (EDA)

Examined class distribution and dataset balance

Analyzed feature characteristics and value ranges

Verified data integrity prior to model training

EDA provided critical insights into the underlying structure of the dataset and guided preprocessing decisions.

🔹 3. Model Development

To ensure a comprehensive evaluation, multiple machine learning algorithms were implemented and compared:

Logistic Regression – baseline linear classifier

Random Forest Classifier – ensemble-based, non-linear model

Support Vector Machine (SVM) – margin-based classifier

The dataset was divided into training and testing subsets to prevent overfitting and ensure fair evaluation.

🔹 4. Model Evaluation & Results

Performance was assessed using standard classification metrics:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

📈 Model Performance Summary
Model	Accuracy
Logistic Regression	100%
Random Forest	100%
SVM	98.75%

Among these, Random Forest was selected as the final model due to its robustness, interpretability, and ability to capture complex feature interactions.

🔹 5. Real-World Prediction System

To enhance practical usability, a custom prediction function was developed that:

Accepts human-readable clinical inputs (e.g., "yes", "no", "normal", "abnormal")

Automatically preprocesses and encodes inputs internally

Outputs an intuitive diagnostic result:

CKD Detected

No CKD Detected

This feature simulates a clinical decision-support tool, bridging the gap between machine learning models and real-world healthcare applications.

🛠️ Technologies Used

Python

Pandas & NumPy

Scikit-learn

Jupyter Notebook / Google Colab

📁 Repository Structure
├── Task1_CKD_Detection.ipynb
├── chronic_kidney_disease.csv
└── README.md

🎯 Key Takeaways

Medical datasets require careful preprocessing and validation

-Model comparison is essential for selecting robust solutions

-Accuracy alone is insufficient — usability and interpretability matter

-Machine learning can effectively augment healthcare diagnostics when applied responsibly