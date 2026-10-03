# Streamlit / Gradio Interactive ML Web App

## Project Overview
This project converts a trained machine learning classifier into an interactive **Streamlit web application**. Users can adjust flower measurements using sliders and immediately receive a predicted flower species and prediction probabilities.

The app uses the Decision Tree model from the previous **First Machine Learning Classifier** project. The trained model is saved with **Joblib**, loaded by the Streamlit application, and used for real-time predictions.

## Key Features
- Streamlit web interface
- Interactive input sliders
- Saved ML model using Joblib
- Real-time prediction
- Prediction probability display
- Clean and beginner-friendly UI
- Reusable trained model
- Deployment-ready project structure

## Machine Learning Model
**Decision Tree Classifier**

Input features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

Output:
- Setosa
- Versicolor
- Virginica

## Project Structure
```text
streamlit_ml_web_app/
├── app/
│   └── app.py
├── data/
│   └── iris_sample.csv
├── model/
│   └── iris_decision_tree.joblib
├── outputs/
├── train_model.py
├── requirements.txt
├── .gitignore
└── README.md
```

## Technologies Used
- Python
- Streamlit
- Scikit-Learn
- Pandas
- Joblib

## Run Locally

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Train/save the model if needed
```bash
python train_model.py
```

### 3. Start the Streamlit app
```bash
streamlit run app/app.py
```

The application will open in your browser.

## Deployment
This project can be deployed using **Streamlit Community Cloud**.

Basic deployment steps:
1. Upload the project to GitHub.
2. Open Streamlit Community Cloud.
3. Select the GitHub repository.
4. Set the main file to `app/app.py`.
5. Deploy the application.

## End-to-End Workflow
```text
Dataset
   ↓
Train Decision Tree
   ↓
Save Model with Joblib
   ↓
Load Model in Streamlit
   ↓
User Enters Values with Sliders
   ↓
Model Predicts Flower Species
   ↓
Prediction + Probability Displayed
```

## Expected Outcome
This project demonstrates how a machine learning model can be converted into a simple interactive web application. It provides practical experience in model serialization, application development, interactive inputs, real-time prediction, and deployment.

## Portfolio Value
The project can be included in a beginner AI/Data Science portfolio because it demonstrates both **machine learning model development** and **web-based model deployment**.

## Author
Student AI / Data Science Project
