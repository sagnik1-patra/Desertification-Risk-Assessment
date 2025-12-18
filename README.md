🌍 Desertification Risk Assessment Using AIS + HSA Hybrid Model
📌 Project Title

Desertification Risk Assessment Using Hybrid AIS–HSA Optimized Support Vector Machine

📖 Project Overview

Desertification is a critical environmental challenge caused by deforestation, climate variability, and unsustainable land use. Early identification of land degradation risk helps policymakers and environmental agencies take preventive actions.

This project proposes a hybrid Artificial Immune System (AIS) + Harmony Search Algorithm (HSA) optimized Support Vector Machine (SVM) model to assess desertification risk using deforestation-related indicators.

The hybrid approach improves prediction stability and avoids local minima by combining global exploration (AIS) with local refinement (HSA).

🎯 Objectives

Analyze deforestation data to estimate land degradation trends

Generate a Desertification Risk Index (0–1 scale)

Optimize SVM hyperparameters using AIS + HSA hybridization

Visualize desertification patterns using graphs and heatmaps

Export results for further analysis and deployment

🧠 Methodology
🔹 Data Source

Dataset: goal15.forest_shares.csv

Domain: Forest cover and deforestation indicators

Source: Kaggle / UN SDG datasets

🔹 Feature Engineering

Forest loss is computed as a proxy for desertification

Risk index normalized between 0 (low risk) and 1 (high risk)

🔹 Machine Learning Model

Algorithm: Support Vector Regression (SVR)

Kernel: Radial Basis Function (RBF)

🔹 Hybrid Optimization Strategy
Algorithm	Role
AIS (Artificial Immune System)	Global search using clonal selection
HSA (Harmony Search Algorithm)	Local refinement using harmony memory
Hybrid AIS → HSA	Robust hyperparameter optimization

Optimized parameters:

C

gamma

epsilon

Parameter bounds are enforced to ensure model stability.

🏗️ System Architecture
Input CSV
   ↓
Data Cleaning & Scaling
   ↓
Feature Engineering
   ↓
AIS Optimization
   ↓
HSA Refinement
   ↓
Optimized SVM Model
   ↓
Risk Prediction
   ↓
Graphs + CSV + JSON Outputs

📂 Project Directory Structure
Desertification Risk Assessment/
│
├── archive/
│   └── goal15.forest_shares.csv
│
├── his_desertification_results.csv
├── his_desertification_predictions.json
│
├── his_accuracy_curve.png
├── his_prediction_comparison.png
├── his_heatmap.png
├── his_prediction_curve.png
│
└── README.md

📊 Outputs Generated
📁 Data Outputs

his_desertification_results.csv
→ Contains original features + predicted risk index

his_desertification_predictions.json
→ Deployment-ready prediction output

📈 Visualization Outputs

Accuracy Curve – Actual vs Predicted values

Prediction Comparison Plot – Regression quality

Correlation Heatmap – Feature relationships

Risk Prediction Curve – Desertification trend

All outputs are saved with the prefix his_.



![Confusion Matrix Heatmap](hybrid_prediction_comparison.png)



📉 Evaluation Metric

Mean Squared Error (MSE)
Used as the fitness function during AIS and HSA optimization.

🧪 Technologies Used

Python 3.10+

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

▶️ How to Run the Project
1️⃣ Install Dependencies
pip install numpy pandas matplotlib seaborn scikit-learn

2️⃣ Update Dataset Path (if needed)
DATA_PATH = r"C:\Users\NXTWAVE\Downloads\Desertification Risk Assessment\archive\goal15.forest_shares.csv"

3️⃣ Run the Script
python ais_hsa_desertification.py


All graphs will:

Display on screen first

Then automatically save in the project folder

🧠 Key Highlights

✔ Hybrid bio-inspired optimization

✔ No external optimization libraries used

✔ Fully reproducible & explainable

✔ Suitable for academic projects, research papers & viva

✔ Easily extendable with NDVI, rainfall, soil moisture data

🧑‍🏫 Viva / Presentation Explanation (Use This)

“The proposed model combines Artificial Immune System for global exploration with Harmony Search Algorithm for local refinement to optimize SVM hyperparameters, resulting in a stable and accurate desertification risk assessment framework.”

🚀 Future Enhancements

Integration of NDVI, rainfall, soil moisture

Geospatial desertification risk maps

Comparison with PSO, CSA, GA hybrids

Deep learning based land degradation modeling

Real-time satellite data integration

📜 License

This project is intended for academic and research purposes.

🙌 Acknowledgements

Kaggle Datasets

UN SDG Environmental Data

Scikit-learn Documentation
