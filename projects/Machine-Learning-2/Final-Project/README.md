# Machine Learning 2 – Final Project

**Course:** Machine Learning 2 (MSDS)  
**Project Type:** Final Project  
**Author:** Learning Team 7

---

## 📌 Overview
This project applies machine learning methods to predict outcomes of the **Volleyball Nations League (VNL)** using detailed team, match, and player-level data from the 2023 season. The goal is to support sports analytics and betting strategies through accurate win–loss and set-level predictions.  

Two predictive pipelines were built:  
- **Bet Smart** – Predicts win/lose outcomes.  
- **Bet Smarter** – Predicts set-level scores.  

Both pipelines include **data scraping, preprocessing, feature engineering, model training with grid search, and interpretability** using SHAP and LIME.

---

## 🧠 Models Used
We evaluated multiple supervised learning classifiers with **Grid Search Cross Validation** to select the best hyperparameters:  

- **Decision Tree Classifier**  
- **Random Forest Classifier**  
- **Gradient Boosting Classifier** ✅ *Best performing model*  
- **K-Nearest Neighbors (KNN)**  
- **Support Vector Classifier (SVC)**  

### Best Models
- **Bet Smart (Win-Loss Prediction)**  
  - GradientBoostingClassifier (max_depth=4, n_estimators=100)  
  - Accuracy: **93.85%** | Precision: **93.10%** | Recall: **95.00%** | F1: **93.66%**  

- **Bet Smarter (Set-Level Prediction)**  
  - GradientBoostingClassifier (max_depth=2, n_estimators=200)  
  - Accuracy: **73.20%** | Precision: **73.80%** | Recall: **71.25%** | F1: **71.67%**  

---

## 🔍 Interpretability
To enhance trust and transparency:  
- **SHAP (SHapley Additive exPlanations):** Global and local feature importance (e.g., player efficiency, performance ranking).  
- **LIME (Local Interpretable Model-agnostic Explanations):** Individual match-level explanations.  

These tools provided insights into why predictions were made, bridging the gap between machine predictions and domain knowledge.

---

## 📊 Results
- **Bet Smart**: High accuracy, reliable for betting win–loss odds.  
- **Bet Smarter**: Lower performance due to multi-class complexity, but valuable for set-level betting strategies.  
- Correctly predicted several June 2024 VNL matches; misses explained by external factors (injuries, strategies not in data).  

---

## 📂 Repository Layout
- `notebooks/ML2_FinalProject.ipynb` → Full pipeline code (scraping, preprocessing, modeling, evaluation).  
- `docs/[LT7 ML2] Final Project.pdf` → Final project report & presentation.  
- `assets/` → Figures, diagrams, and pipeline visuals.  
- `data/` → Processed VNL datasets (CSV).  

---

## 🚀 Business Value
- **Teams & Coaches:** Data-driven insights into performance metrics.  
- **Bettors:** Transparent, interpretable predictions to guide betting strategies.  
- **Betting Platforms:** Competitive edge through predictive analytics for customer engagement and retention.  


