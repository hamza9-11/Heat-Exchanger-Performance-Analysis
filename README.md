# Heat Exchanger Performance Prediction using Machine Learning

## Project Overview
In the petroleum refining industry, sensor data is often noisy, making it difficult to accurately predict equipment performance. This project aims to build a robust Machine Learning model to predict the **Heat Load** of a heat exchanger using noisy input data (Temperature & Flow Rate), simulating real-world refinery conditions.

## Methodology
1. **Baseline Model:** Trained a Linear Regression model on clean simulation data to establish theoretical physics.
2. **Real-world Simulation:** Tested the model on noisy data (simulating sensor errors) after applying IQR outlier removal.
3. **Advanced Modeling:** Implemented a **Random Forest Regressor** to capture non-linear relationships and improve resistance to noise.

## Key Findings
- The theoretical maximum R² score for this noisy dataset is approximately **0.57** (due to the high aleatoric uncertainty/noise ratio).
- The Linear Regression model underperformed on noisy data.
- The **Random Forest model achieved an R² score of ~0.50**, successfully capturing the physical patterns despite the heavy noise, proving its robustness for industrial applications.

## Tools Used
- Python (Pandas, NumPy, Scikit-Learn)
- Data Visualization (Matplotlib, Seaborn)

## Dataset Source
The dataset used in this project is publicly available on Kaggle:
Heat Exchanger Dataset : Parametric Study([KAGGLE_DATASET_LINK](https://www.kaggle.com/datasets/kuriangeorge/heat-exchanger-dataset-parametric-study))
