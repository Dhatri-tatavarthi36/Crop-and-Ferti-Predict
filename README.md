# Crop-and-Ferti-Predict
# 🌾 Crop and Fertilizer Prediction System

This project uses **machine learning** to recommend the most suitable **crop** and **fertilizer** based on soil nutrients (N, P, K), environmental factors (temperature, pH, rainfall), and intelligent rule-based nutrient analysis.

---

## 🔍 Project Overview

### ✅ Features:
- **Crop Prediction** using Random Forest Classifier
- **Fertilizer Prediction** using Multiclass Classification
- **Rule-Based NPK Level Analysis**: Additional advice on increasing/decreasing N, P, K
- **Runtime Input Support** from users (terminal-based)

---

## 📂 Dataset Structure

The dataset used contains the following columns:

| N | P | K | temperature | ph | rainfall | Crop | Fertilizer |
|---|---|---|-------------|----|----------|------|------------|

- **N, P, K**: Soil nutrients
- **temperature**: Measured in °C
- **ph**: Soil pH value
- **rainfall**: Annual rainfall (mm)
- **Crop**: Crop suitable for the given conditions
- **Fertilizer**: Recommended fertilizer for that crop


---

## 🧠 Models Used

1. **Crop Prediction Model**
   - Algorithm: `RandomForestClassifier`
   - Input Features: N, P, K, temperature, ph, rainfall
   - Target: Crop (multiclass)

2. **Fertilizer Prediction Model**
   - Algorithm: `RandomForestClassifier`
   - Input Features: N, P, K, temperature, ph, rainfall, predicted_crop
   - Target: Fertilizer (multiclass)

3. **Rule-Based NPK Analysis**
   - Compares user’s NPK values with ideal values
   - Provides recommendations like:
     - "Increase Nitrogen"
     - "Decrease Potassium"
     - or "NPK levels are optimal."

---
