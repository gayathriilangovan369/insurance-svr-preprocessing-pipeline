# Insurance SVR Preprocessing Pipeline

This project predicts insurance charges using Support Vector Regression (SVR).  
The focus is on understanding how preprocessing affects model performance.

---

## Project Overview

This project implements SVR using two approaches:

1. **Input preprocessing only**
   - Applied StandardScaler to input features  

2. **Input and output preprocessing**
   - Applied StandardScaler to both input (X) and output (y)  
   - Used inverse transformation to get the final output  

---

## Workflow

Basic approach:  
Input → Scaling → SVR Model → Prediction → Output  

Advanced approach:  
Input → Scaling → SVR Model → Prediction → Inverse Scaling → Final Output  

---

## Project Structure

### notebooks
- 01_svr_input_preprocessing.ipynb  
- 02_svr_input_output_preprocessing.ipynb  

### models
- insurance_svr_model.sav  
- insurance_input_scaler.sav  
- insurance_output_scaler.sav  

### data
- insurance_pre.csv  

---

## Technologies Used

- Python  
- Pandas  
- Scikit-learn  
- Support Vector Regression (SVR)  

---

## Key Concepts

- Feature scaling using StandardScaler  
- Output scaling and inverse transformation  
- Model training and prediction  
- Saving and loading model using pickle  
- Pipeline-based workflow  

---

## Conclusion

Scaling both input and output improves the performance of SVR compared to scaling only the input.  
This project demonstrates how proper preprocessing can enhance model accuracy and stability.
