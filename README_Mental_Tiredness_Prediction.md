# 🧠 Mental Tiredness Score Predictor

A Streamlit web app that predicts a person's mental tiredness score based on their work habits, sleep, lifestyle, and environment — and gives personalised tips to reduce fatigue.

## 📌 Overview

This project uses a **Ridge Regression** model (Test R² = 0.75) trained with **scikit-learn**, **MLflow**, and **Optuna** to estimate a mental tiredness score (0–100) from daily lifestyle and work-related inputs. The app is built with **Streamlit** and gives instant predictions plus actionable recommendations.

## ✨ Features

- Interactive input form covering:
  - Work & cognitive load (decisions made, context switches, notifications, workload)
  - Screen time, deep work minutes, task complexity, breaks
  - Sleep, hydration, caffeine intake
  - Mood, work type, and work environment
- One-click prediction with a visual score bar
- Colour-coded tiredness level (Low / Moderate / High)
- Personalised tips based on your inputs (sleep, caffeine, hydration, breaks, screen time)

## 🛠️ Tech Stack

- Python
- Streamlit
- scikit-learn
- Pandas / NumPy
- Joblib (model loading)
- MLflow & Optuna (used during model training/tuning)

## 📂 Project Structure

```
Mental_tirdness_ML_FLOW/
├── app.py              # Streamlit app
├── model.pkl           # Trained Ridge Regression model
├── requirements.txt    # Python dependencies
└── README.md
```

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/gopivallepu41/Mental_tirdness_ML_FLOW.git
cd Mental_tirdness_ML_FLOW
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the app
```bash
streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`.

## 🧪 How It Works

1. Enter your work, sleep, and lifestyle details in the form.
2. Click **⚡ Predict Mental Tiredness Score**.
3. The app runs your inputs through the trained model and returns:
   - A predicted tiredness score (0–100)
   - A tiredness level (🟢 Low / 🟡 Moderate / 🔴 High)
   - Personalised tips to help you recover or maintain good habits

## 📊 Model

- **Algorithm:** Ridge Regression
- **Test R²:** 0.75
- **Tracked with:** MLflow
- **Hyperparameter tuning:** Optuna

## 🔮 Future Improvements

- Add model retraining pipeline
- Track prediction history per user
- Deploy with authentication for personalised long-term tracking

## 📄 License

This project is open-source and available for learning and demonstration purposes.
