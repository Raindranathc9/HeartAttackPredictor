# HeartAttackPredictor

This project involves developing a machine learning model to predict the likelihood of a heart attack based on various health parameters.

## Project Overview

The heart attack prediction model is designed to analyze medical data and provide predictions to assist in early diagnosis and preventive healthcare measures. 

## Dataset

The dataset includes the following features:
- **age**: Age of the patient
- **anaemia**: Presence of anaemia (0: No, 1: Yes)
- **creatinine phosphokinase**: Level of creatinine phosphokinase in the blood
- **diabetes**: Presence of diabetes (0: No, 1: Yes)
- **ejection fraction**: Percentage of blood leaving the heart each time it contracts
- **high bp**: Presence of high blood pressure (0: No, 1: Yes)
- **platelets**: Platelet count in the blood
- **serum creatinine**: Level of serum creatinine in the blood
- **serum sodium**: Level of serum sodium in the blood
- **sex**: Gender of the patient (0: Female, 1: Male)
- **smoking**: Smoking status (0: No, 1: Yes)
- **death**: Outcome (0: No, 1: Yes)

## Requirements

To run the model, ensure you have the following libraries installed:

- `joblib`
- `numpy`
- `pandas`
- `scikit-learn` (if using a model from this library)

You can install these libraries using pip:

```bash
pip install joblib numpy pandas scikit-learn
