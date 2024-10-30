# How to Use the Heart Attack Predictor
Load the Model
Ensure you have your trained model saved as a .pkl file. Use the following code snippet to load your model:

python
Copy code
import joblib

# Load the model (replace 'your_model_filename.pkl' with the actual model filename)
model = joblib.load('your_model_filename.pkl')
Prepare Input Features
Prepare your input data as a NumPy array. Make sure that the input shape matches the features used during model training. Here’s an example:

python
Copy code
import numpy as np

# Sample input features
features = np.array([[62, 0, 61, 1, 38, 1, 155000, 1.1, 143, 1, 1]])
Feature Format:

  age: Age of the patient (e.g., 62)
  anaemia: 1 if the patient has anaemia; otherwise, 0
  creatinine phosphokinase: CPK enzyme level
  diabetes: 1 if the patient has diabetes; otherwise, 0
  ejection fraction: Percentage of blood leaving the heart per beat
  high bp: 1 if the patient has high blood pressure; otherwise, 0
  platelets: Platelet count
  serum creatinine: Level of serum creatinine in the blood
  serum sodium: Level of serum sodium in the blood
  sex: 1 for male, 0 for female
  smoking: 1 if the patient smokes; otherwise, 0
Make Predictions
Use the loaded model to make predictions based on the prepared features.

  # Make a prediction
  
  prediction = model.predict(features)
  print("Prediction:", "Heart Attack Risk" if prediction[0] == 1 else "No Heart Attack Risk")
  
Output Interpretation:
1: Indicates a higher risk of a heart attack.
0: Indicates a lower or no risk of a heart attack.
