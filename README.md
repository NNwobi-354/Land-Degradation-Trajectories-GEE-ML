# Land Degradation Trajectories in the Nigerian Sahel and Russian Steppe (2000–2025)

## 📌 Project Overview
This repository contains the comprehensive analytical pipeline for a comparative study assessing the drivers of land degradation across two distinct ecological regimes: the **Nigerian Sahel** and the **Russian Steppe**. By leveraging **Google Earth Engine (GEE)** and **Machine Learning (Random Forest & XGBoost)**, this research identifies how environmental variables and social factors (such as conflict) interact to drive vegetation decline over a 25-year trajectory.

## 🧪 Scientific Methodology
The study utilizes a multi-stage approach to quantify degradation:
*   **Data Acquisition**: High-resolution satellite imagery and 13 environmental/social predictors including Albedo, Soil Moisture, and Conflict Density.
*   **Trend Analysis**: Application of the **Mann-Kendall trend test** and **NDVI anomalies** to identify "Crisis Years" of significant browning.
*   **Machine Learning Attribution**: Using **Random Forest** and **XGBoost** to rank driver importance via Mean Decrease in Impurity (MDI).
*   **Statistical Validation**: Robustness checks using **Variable Influence on Projection (VIP)** and **Z-score extremity analysis**.

## 📂 Repository Structure
*   `data/`: Contains `Nigeria_Long_Format.csv` and `Russia_Long_Format.csv`.
*   `scripts/`: Python scripts for Sections 4.1 through 4.6, covering model training, validation, and regime signature analysis.
*   `figures/`: High-resolution (700 DPI) publication-ready visualizations, including:
    *   **Figure 7**: Observed vs. Predicted Model Validation.
    *   **Figure 8**: Comparative Driver Rankings.
    *   **Figure 9/10**: Radar Signatures and Mirror Divergence Plots.
    *   **Figure 11/12**: Anomaly Timelines and Interaction Bubble Plots.
    *   **Figure 13/14**: VIP Significance and Z-Score Robustness.

## 🚀 Key Findings
*   **Regime Divergence**: Nigeria's degradation is heavily influenced by **Social Conflict** and **Surface Albedo**, whereas Russia's landscape is primarily sensitive to **Wind Speed** and **Soil Moisture**.
*   **Model Accuracy**: Both Random Forest and XGBoost models achieved high predictive reliability ($R^2 > 0.85$) across both study areas.
*   **Spatio-Temporal Anomalies**: Statistically significant browning events ($p < 0.05$) were successfully mapped to specific drought and conflict-intensive years.

## 🛠 How to Use
1.  **Clone the Repository**:
    ```bash
    git clone [https://github.com/NNwobi-354/Land-Degradation-Trajectories-GEE-ML.git](https://github.com/NNwobi-354/Land-Degradation-Trajectories-GEE-ML.git)
    ```
2.  **Install Dependencies**:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn xgboost
    ```
3.  **Run Analysis**: Execute the provided Python scripts in sequence to generate the metrics and figures presented in the thesis.

## 🎓 Citation & Contact
**Author**: Nwobi et al., 2026  
**Program**: Planet Education and Research Program  
**Date**: May 2026

---
*This research was supported by satellite data provided through the Planet Education and Research Program.*
