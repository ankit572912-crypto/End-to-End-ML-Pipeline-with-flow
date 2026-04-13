# End-to-End-ML-Pipeline-with-flow
End-to-End Machine Learning Pipeline with MLflow & FastAPI

This project demonstrates a complete production-ready ML workflow including data generation, model training, experiment tracking, and API deployment.

📌 Project Overview
Generate synthetic dataset
Train a Machine Learning model (Random Forest)
Track experiments using MLflow
Serve predictions via FastAPI
Enable reproducibility and scalability
🧠 Tech Stack
Python
Scikit-learn
MLflow
FastAPI
Pandas, NumPy
Uvicorn
📂 Project Structure
├── data/
│   └── data.csv
├── generate_data.py     # Generates dataset
├── train.py             # Model training + MLflow logging
├── predict.py           # Load model & predict
├── app.py               # FastAPI deployment
├── requirements.txt
└── README.md
⚙️ Setup Instructions
1. Clone the Repository
git clone https://github.com/your-username/your-repo.git
cd your-repo
2. Install Dependencies
pip install -r requirements.txt
📊 Step 1: Generate Dataset
python generate_data.py

✔ Creates synthetic dataset with features:

Age
Salary
Experience
Education Level
City Tier
🏋️ Step 2: Train Model
python train.py

✔ Trains Random Forest Classifier
✔ Logs experiments in MLflow
✔ Saves model artifact

📈 Step 3: Run MLflow UI
mlflow ui

Open in browser:

http://127.0.0.1:5000
🔮 Step 4: Make Predictions (Script)
python predict.py
🌐 Step 5: Run FastAPI Server
uvicorn app:app --reload

Visit:

http://127.0.0.1:8000
API Endpoints
/ → Health Check
/predict → Returns prediction
📌 Sample Prediction Input
[30, 60000, 5, 1, 2]
