# Intelligent Modeling and Optimization of Blood Products Stock Management

This project combines stochastic Petri Net modeling and machine learning to optimize blood product inventory management at the Blood Transfusion Center (CWTS) of Béjaïa, Algeria. It addresses the critical challenge of managing blood products with limited shelf life and variable demand, achieving a service rate improvement from 31.86% to 81.30%.

## Objective

To optimize blood product inventory management by:
- Modeling system dynamics using Stochastic Petri Nets (RdPSG)
- Predicting monthly demand using ensemble machine learning
- Establishing data-driven reorder points and safety stock policies
- Providing operational decision support through an interactive dashboard
- Improving service rate from 31.86% to 81.30%

## Data

Real-world dataset from CWTS Béjaïa (confidential):
- 48 months of historical records
- 3 blood product types: Erythrocyte Concentrates (CE), Platelet Concentrates (CPS), Fresh Frozen Plasma (PFC)
- 4,800+ transactions
- Note: Data is not included in this repository due to confidentiality agreements

## Methodology

**Stochastic Petri Net (RdPSG):**
- Formal modeling of blood product flow (arrival → testing → storage → distribution → expiration)
- Steady-state analysis via Markov chains
- Performance evaluation on system dynamics

**Machine Learning Models:**
- CatBoost (Gradient Boosting) : 5.54% MAPE
- XGBoost (Extreme Gradient Boosting) : 12.96% MAPE
- Random Forest (Tree Ensemble) : Stability evaluation
- Time-series features with explanatory variables

**Performance Metrics:**
- Mean Absolute Percentage Error (MAPE)
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Service rate improvement: 31.86% → 81.30%

## Repository Content

- **README.md**
- **Full Thesis.pdf**: Complete thesis with full methodology and results
- **Project_Leaflet.pdf**: Visual summary of the project
- **dashboard_screenshot.png**: Preview of the interactive dashboard


## Key Results

| Metric | Before | After | Impact |
|--------|--------|-------|--------|
| Service Rate (CE) | 31.86% | 81.30% | +156% improvement |
| Stockout Probability | Baseline | 68.14% | Reduced (nominal conditions) |
| Best ML Model (MAPE) | — | 5.54% | CatBoost |


## Notes

- Code and data are confidential and not included in this repository. Researchers can request access through CWTS Béjaïa or thesis advisors (Pr. Ouiza Lekadir, Mr. Ramzi Sahli)
- File paths in notebooks may need adjustment for your environment
- Complete methodology, results, and analysis are detailed in `Full Thesis.pdf`
- Dashboard requires a modern web browser (Chrome, Firefox, Safari, Edge)

## Authors

**Dahmani Mahdi** & **Chamen Rayane**

Master 2  Applied Mathematics (Data Science & Decision Support)  
Université Abderrahmane Mira, Béjaïa, Algeria

**Advisors**: Pr. Ouiza Lekadir, Mr. Ramzi Sahli  
**Institution**: Centre de Wilaya de Transfusion Sanguine (CWTS), Béjaïa
