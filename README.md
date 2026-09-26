# Healthcare Multi-Disease Prediction System

This project provides a Machine Learning based system for predicting the risk of multiple diseases including **Heart Disease**, **Diabetes**, and **Breast Cancer**.  
The system uses medical parameter inputs provided by the user and classifies whether the person is likely to have the specific disease or not.

## 1. Introduction

Healthcare diagnosis using machine learning helps in early prediction of diseases which can save lives.  
This project trains **separate ML models** for three diseases and integrates them into one user-friendly interface.

The diseases covered are:
- Heart Disease
- Diabetes
- Breast Cancer

## 2. Technologies Used

| Category | Tools / Libraries |
|---------|------------------|
| Programming Language | Python |
| ML Framework | Scikit-Learn |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| User Interface | Streamlit / Tkinter |

## 3. Project Structure

```
├── medical_diagnosis_UI.py         # Streamlit / UI Application
├── Heart.ipynb                     # Model training for Heart Disease
├── Diabeties.ipynb                 # Model training for Diabetes
├── Breast-Cancer.ipynb             # Model training for Breast Cancer
├── heart.csv                       # Heart dataset
├── diabetes.csv                    # Diabetes dataset
├── breast-Cancer.csv               # Breast Cancer dataset
├── saved_models/                   # Trained model files (.sav)
├── requirements.txt                # Required dependencies
└── README.md                       # Project documentation
```

## 4. Datasets

| Disease | File | Source | Description |
|--------|------|--------|-------------|
| Heart Disease | `heart.csv` | UCI Repository | Contains patient heart-related measurements |
| Diabetes | `diabetes.csv` | UCI/Kaggle | Includes blood glucose and medical attributes |
| Breast Cancer | `breast-Cancer.csv` | UCI/Kaggle | Features mass/shape measurements for cancer detection |

## 5. Model Workflow

1. Load dataset
2. Handle missing values and apply scaling
3. Split dataset into train and test sets
4. Train ML models (Logistic Regression / Random Forest / SVM)
5. Evaluate model performance
6. Save trained model files using pickle (.sav)
7. Predict disease in UI using user input values

## 6. How to Run the Project

### Option 1: Run the Desktop Python UI
```
python medical_diagnosis_UI.py
```

### Option 2: Run the Streamlit Web Application

#### Step 1: Install Streamlit (if not installed)
```
pip install streamlit
```

#### Step 2: Run the Streamlit app
```
streamlit run medical_diagnosis_UI.py
```

Once the server starts, the app will open automatically in your browser.

## 7. Results (Accuracy)

| Disease Model | Algorithm Used | Approx Accuracy |
|---------------|----------------|----------------|
| Heart Disease | Logistic Regression / Random Forest | ~80–90% |
| Diabetes | SVM / Logistic Regression | ~75–85% |
| Breast Cancer | Random Forest / SVM | ~90–95% |

*(Accuracy values may vary depending on training settings.)*

## 8. Future Enhancements

- Deploy web version to cloud (Render / Streamlit Cloud / AWS)
- Add more disease modules
- Build mobile application for easy usage
- Store medical records in database

## 9. Acknowledgements

- UCI Machine Learning Repository
- Kaggle Dataset Contributors
- Scikit-learn & Python Community

## 10. Author

<!-- **Mohammed Furqan**   -->
Final Year Project — AI & ML
