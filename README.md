# Human Cognitive Performance Prediction

This project explores whether behavioral and lifestyle variables—such as sleep duration, stress level, caffeine intake, and working-memory accuracy—can predict cognitive performance, measured using **Stroop Task Reaction Time**. 

The analysis uses the Kaggle dataset *Sleep Deprivation and Cognitive Performance* and implements a full machine-learning workflow including preprocessing, visualization, model tuning, and evaluation.

---

## Project Objectives
- Understand how sleep, stress, and lifestyle metrics relate to cognitive performance.
- Perform exploratory data analysis (EDA) using histograms, scatterplots, and correlation heatmaps.
- Build and evaluate multiple ML models, including:
  - Linear Regression  
  - Random Forest  
  - Gradient Boosting  
  - K-Nearest Neighbors (KNN)
- Use GridSearchCV to tune the KNN model.
- Compare predictive performance using MSE, MAE, and R².

---

## Findings
- **KNN showed the lowest error (best performance),** but all models produced negative R² values.
- This indicates the models could not outperform a simple average predictor—however, this is *common in cognitive and behavioral datasets*, where human performance is highly variable.
- Sleep, stress, caffeine intake, and working-memory accuracy showed **weak predictive power** for Stroop reaction time in this sample.
- Results highlight the complexity of modeling human cognition with simple behavioral measures.

---

## Dataset
Source: Kaggle  
https://www.kaggle.com/datasets/sacramentotechnology/sleep-deprivation-and-cognitive-performance/data

This dataset includes:
- Sleep Hours  
- Sleep Quality Score  
- Daytime Sleepiness  
- Stress Level  
- N-Back Accuracy  
- Emotion Regulation Score  
- PVT Reaction Time  
- Stroop Reaction Time  
- Caffeine Intake  
- Physical Activity Level  
- BMI  
- Age  
- Gender  

Raw data is **not included** in the repo—only referenced.

---

## Notebook
The full analysis is located in:

```
human_cognitive_performance.ipynb
```

It includes:
1. Data Cleaning & Preprocessing  
2. Exploratory Data Analysis  
3. KNN Hyperparameter Tuning  
4. Model Training & Evaluation  
5. Final Model Comparison  
6. Visualizations (Actual vs Predicted, pairplots, etc.)

---

## Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
```

Install with:

```bash
pip install -r requirements.txt
```

---

## How to Run

Clone the repo:

```bash
git clone https://github.com/<your-username>/Human-Cognitive-Performance.git
cd Human-Cognitive-Performance
```

Launch the notebook:

```bash
jupyter notebook notebooks/human_cognitive_performance.ipynb
```

---

## Conclusion

This project demonstrates the challenges of predicting human cognitive performance using behavioral variables. While the models did not achieve strong predictive power, the workflow provides a full example of real-world data preprocessing, visualization, and machine-learning evaluation on a noisy behavioral dataset.

---
