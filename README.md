# Liver Cirrhosis Risk Prediction Web App

## Project Summary
This project is a machine learning-powered web application that predicts the risk of liver cirrhosis in patients using clinical and blood test data. It features a user-friendly Flask web interface for healthcare professionals to input patient data and receive real-time predictions based on a trained XGBoost model.

---

## Features
- Real-time liver cirrhosis risk prediction
- Clean, web-based input form for medical data
- Data-driven, binary prediction output (Cirrhosis/No Cirrhosis)
- Uses a cleaned and preprocessed medical dataset
- Achieved 100% accuracy on test data (on available dataset)

---

## Dataset Overview
The dataset includes features such as:
- Age, Alcohol Consumption (duration and quantity)
- Hemoglobin, PCV, MCV, Total Count, Polymorphs, Lymphocytes, Monocytes, Eosinophils, Basophils
- Platelet Count, Direct/Indirect Bilirubin, Total Protein, Albumin, Globulin
- AL Phosphatase, SGOT/AST, SGPT/ALT
- **Target column:** `Predicted Value` (0 = Cirrhosis, 1 = No Cirrhosis)

All non-numeric features (like gender, place, alcohol type, etc.) are removed except the target variable.

---

## Tech Stack
| Component  | Technology         |
|------------|--------------------|
| ML Model   | XGBoost            |
| Backend    | Python + Flask     |
| Frontend   | HTML (vanilla)     |
| Tools      | Jupyter Notebook   |
| Dataset    | CSV Format         |

---

## Project Structure
```
project_root/
│
├── app.py                  # Flask web application
├── model_training.ipynb    # Jupyter notebook for data cleaning, training, and model export
├── cirrhosis_model.pkl     # Trained XGBoost model
├── HealthCareData.csv      # Cleaned dataset
├── requirements.txt        # Python dependencies
├── templates/              # HTML templates (index.html, result.html)
├── Document/               # Project documentation (PDFs)
├── Demo_media/             # Demo images and demo_video.mp4
└── README.md               # Project documentation
```

---

## How to Run the Project

### Prerequisites
- Python 3.11+
- Flask
- pandas, numpy, scikit-learn, xgboost, joblib

### Setup Instructions
```bash
# Clone the repository
# cd into the project directory
pip install -r requirements.txt
python app.py
```

---

## Usage
1. Open your browser and go to `http://127.0.0.1:5000/`
2. Enter patient data in the form and submit.
3. View the prediction result (Cirrhosis/No Cirrhosis).

---

## Notes
- The model was trained on a cleaned dataset and may not generalize to all populations.
- For demo purposes only. Not for clinical use.

---

## Authors & Credits
- Original dataset: Kaggle
- Project contributors: [Your Name Here]

## requirements.txt

```
Flask
pandas
numpy
scikit-learn
xgboost
joblib
```
