# How to Use the Heart Attack Predictor

1. Load the Model:
   Ensure you have your trained model saved as a .pkl file. Use the following code snippet to load your model:
   
   import joblib
   
   model = joblib.load('your_model_filename.pkl')  # Replace with your actual model filename

2. Prepare Input Features:
   Prepare your input data as a NumPy array. Ensure that the input shape matches the features used during model training:
   
   import numpy as np
   
   # Sample input features
   features = np.array([[62, 0, 61, 1, 38, 1, 155000, 1.1, 143, 1, 1]])

3. Make Predictions:
   Use the loaded model to make predictions based on the prepared features:
   
   prediction = model.predict(features)
   print("Prediction:", prediction[0])  # Output: 0 or 1
