🛡️ Fraud Detection System using Django
This project is a web-based Fraud Detection System developed using the Django framework. It aims to identify and flag suspicious transactions or activities using machine learning models integrated into a Django web application.

🔍 Features
User authentication: Secure login/signup for users and admins.

Upload transactions: Upload datasets (CSV) or input transactions manually.

Fraud prediction: Predict whether a transaction is fraudulent using a trained ML model.

Dashboard: Admin panel to view total transactions, flagged frauds, and user activity.

Visualization: Graphs and tables to summarize prediction outcomes.

🧠 Machine Learning Integration
A pre-trained ML model (e.g., Logistic Regression, Random Forest, or XGBoost) is used to predict fraudulent transactions. The model is loaded using joblib or pickle and invoked through Django views.

📁 Project Structure

fraud_detection/
├── fraud_detection/       # Main Django project
│   ├── settings.py        # Project settings
│   └── urls.py            # URL routing
├── detector/              # Core app for fraud detection
│   ├── models.py          # DB models
│   ├── views.py           # Logic to process requests
│   ├── urls.py            # App-specific URLs
│   └── templates/         # HTML templates
├── static/                # CSS, JS, images
├── ml_model/              # Trained model file (.pkl or .joblib)
└── manage.py
