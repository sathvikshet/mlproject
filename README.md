 🎓 Student Exam Performance Prediction System

This project is an end-to-end Machine Learning pipeline with a Flask web application that predicts students’ math exam scores based on their demographic and academic attributes.

It covers data ingestion, transformation, model training, evaluation, and deployment with a clean modular architecture.



Features
- Data Ingestion: Reads raw CSV, splits into train/test sets, stores artifacts. 
 
- Data Transformation: Handles missing values, encoding, and scaling using `Pipeline` & `ColumnTransformer`.  

- Model Training: Trains multiple ML models (Linear Regression, Random Forest, XGBoost, CatBoost, AdaBoost, etc.) with GridSearchCV for hyperparameter tuning.  

- Model Selection: Automatically selects the best-performing model based on R² score.  

- Prediction Pipeline: Loads saved model & preprocessor to serve real-time predictions.
  
- Flask App UI: User-friendly interface to input details and get predicted math scores instantly.  


⚙️ Tech Stack


- Python, Flask – Web framework  
- Scikit-learn, CatBoost, XGBoost – ML   algorithms  
- Pandas, NumPy, Matplotlib, Seaborn – Data analysis & visualization  
- GridSearchCV – Hyperparameter tuning  
- Pickle/Dill– Model persistence  


📊 Workflow
1.Data Ingestion → Load CSV → Train-Test split → Save artifacts  
2.Data Transformation→ Imputation → Encoding → Scaling → Save preprocessor  
3.Model Training → Train multiple regressors → Hyperparameter tuning → Select best model → Save  
4.Prediction Pipeline → Load model + preprocessor → Transform new data → Predict  
5.Deployment → Flask app with input form for predictions  



 🖥️ To Run the Project:
 Clone the repo

git clone https://github.com/your-username/studentstudent-exam-performanc

cd student-exam-performance



Install dependencies:

pip install -r requirements.txt


Run Flask  App:

python app.py



DEMO:
Enter student details (gender, parental education, lunch type, test prep, scores).

Click Predict → The model predicts Math Score in real-time.
