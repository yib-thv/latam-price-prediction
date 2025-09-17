# latam-price-prediction
# Latam Price Prediction
## Predictive Airfare & Multi-Objective Analysis Based on Machine Learning

This project focuses on **predicting airline ticket prices for domestic flights in Peru (Latam Airlines)**, helping users identify the **optimal time to purchase tickets** for cost savings, comfort, and travel efficiency. The repository implements multi-objective prediction models and comparative analysis of classical and neural network models.

---

## Project Overview

The project performs:

1. **Exploratory Data Analysis (EDA)**  
   - Visualization of trends and distributions in ticket prices, flight schedules, and booking behavior.
   - Preprocessing including normalization to handle outliers.

2. **Data Transformation**  
   - **One-hot encoding**  
   - **Embedding-based encoding**  

3. **Predictive Modeling**  
   - **Eight models trained:** 4 classical (e.g., Decision Tree, Random Forest, KNN, XGBoost) and 4 neural network models (e.g., LSTM, GRU, TCN, Transformer).  
   - Hyperparameter optimization using **Optuna**.  

4. **Evaluation Metrics**  
   - **R²** for regression tasks.  
   - **F1-score** for classification tasks.  
   - Classical models are faster and suitable for resource-limited environments.  
   - Neural networks achieve higher precision but require more computation time.

---

## Objectives

1. **Predict ticket prices** (Objective 1).  
2. **Predict optimal days in advance** to purchase a ticket (Objective 2).  
3. **Predict the most favorable flight time range** (Objective 3).  
4. **Joint prediction of Objectives 1, 2, and 3** (multi-output prediction) (Objective 4).  

---

## Repository Structure

/notebooks/ → Jupyter notebooks for EDA and analysis
/scripts/ → Python scripts for prediction models (Objectives 1, 2, 3 and 4 for each type of data transformation with One-hot encoding and Embedding-based encoding )
/README.md → Project documentation
/requirements.txt → Python dependencie


---

## Features

- **Exploratory Analysis:** Insights into ticket pricing trends and patterns.  
- **Multi-Objective Prediction:** Supports individual objectives and joint multi-output prediction.  
- **Flexible & Modular Code:** Easy to incorporate new models, analyses, and future objectives.  

---

## Requirements

- **Python:** 3.10+  
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn, jupyter  


## How to Run

1. Clone the repository:

git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git

2. Install required libraries:

pip install -r requirements.txt


3. Run notebooks (example):

jupyter notebook notebooks/data_exploration_initial.ipynb
jupyter notebook notebooks/latam_price_analysis.ipynb


4. Run prediction scripts (example):

python scripts/prediction_objective_1_multi_E.py
python scripts/latam_price_prediction.py