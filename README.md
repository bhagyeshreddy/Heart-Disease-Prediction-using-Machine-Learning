# Heart-Disease-Prediction-using-Machine-Learning

## Overview
Heart failure is one of the leading causes of death globally. Early detection is critical for improving patient outcomes and reducing healthcare costs. This project leverages machine learning models to predict heart failure based on clinical and demographic data, enabling accurate and rapid screening to support healthcare professionals in decision-making.

## Business Context
- **Problem**: Heart failure diagnostic processes can be time-consuming and costly. There is a need for rapid, accurate, and affordable diagnostic tools.
- **Objective**: Develop machine learning models for early detection of heart failure to improve patient outcomes, optimize resource allocation, and support preventive healthcare initiatives.

## Features and Insights
1. **Data Analysis**:
   - Demographics: Men show higher prevalence of heart disease (58%) compared to women (42%).
   - Age is a significant factor, with risk increasing after age 50, peaking between 55-65 years.
   - Clinical patterns: Chest pain types, ST slope, and exercise-induced angina strongly correlate with heart disease.

2. **Key Predictors**:
   - ST Slope (28% importance)
   - Exercise Angina (22% importance)
   - Chest Pain Type (18% importance)
   - Age (12% importance)
   - Maximum Heart Rate (10% importance)

3. **Machine Learning Models**:
   - Logistic Regression: Accuracy 85.87%, F1-Score 0.87
   - Random Forest: Accuracy 90.76%, F1-Score 0.92

## Technical Implementation
- **Data Preprocessing**:
  - Addressed class imbalance using SMOTE (Synthetic Minority Oversampling Technique).
  - Normalized features using StandardScaler for consistency.
  - Eliminated multicollinearity with Variance Inflation Factor (VIF).

- **Models Used**:
  - Logistic Regression for interpretability.
  - Random Forest for higher accuracy and feature importance analysis.

- **Evaluation Metrics**:
  - Accuracy, Precision, Recall, F1-Score, and ROC Curve were used to assess model performance.

## Business Impact
- **Early Screening**: AI-driven tools can enable early detection and intervention.
- **Resource Optimization**: Models can guide healthcare providers in prioritizing high-risk patients.
- **Preventive Care**: Insights can help target high-risk groups with personalized preventive campaigns.
- **Accessibility**: Promotes affordable and scalable diagnostics in underserved areas.

## Data
The dataset includes clinical and demographic features:
- **Age**: Patient age (years).
- **Sex**: Male (M) or Female (F).
- **Chest Pain Type**: Typical Angina (TA), Atypical Angina (ATA), Non-Anginal Pain (NAP), Asymptomatic (ASY).
- **Resting BP**: Resting blood pressure (mm Hg).
- **Cholesterol**: Serum cholesterol (mg/dl).
- **Fasting Blood Sugar**: Binary (1 if > 120 mg/dl, 0 otherwise).
- **Resting ECG**: Normal, ST-T wave abnormality, or left ventricular hypertrophy.
- **Max Heart Rate**: Maximum heart rate achieved.
- **Exercise Angina**: Binary (Yes or No).
- **Oldpeak**: ST depression induced by exercise.
- **ST Slope**: Slope of peak exercise ST segment (Up, Flat, Down).
- **Heart Disease**: Binary output class (1: Heart disease, 0: Normal).

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/heart-failure-prediction.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Heart_Failure_Prediction.ipynb
   ```
4. Execute the cells to preprocess the data, train models, and evaluate results.

## Results
- **Logistic Regression**:
  - Accuracy: 85.87%
  - Precision: 0.87
  - Recall: 0.88
  - F1-Score: 0.87

- **Random Forest**:
  - Accuracy: 90.76%
  - Precision: 0.91
  - Recall: 0.92
  - F1-Score: 0.92

## Files
- `Heart_Failure_Prediction.ipynb`: Jupyter notebook with complete analysis and implementation.
- `data/`: Contains the dataset used for model training and testing.
- `README.md`: Project overview and instructions.

## Business Recommendations
- **Early Screening Programs**: Deploy AI tools for high-risk groups.
- **Diagnostic Support**: Use Random Forest models for accurate predictions.
- **Resource Allocation**: Optimize hospital workflows using predictive insights.
- **Preventive Campaigns**: Focus on targeted health initiatives.

## Dependencies
- Python 3.x
- pandas, numpy, scikit-learn, matplotlib, seaborn

## Acknowledgments
This project was developed as part of the SCH-MGMT 657 course by Group 2:
- Bhagyesh Reddy Bheemireddy
- Rupali Madishetty
- Chaitanya Krishna Chaluvadi
- Surya Gande
- Alistair Michael
