# Crop Recommendation System using Machine Learning

A machine learning–powered system that recommends the **most suitable crop** to cultivate based on soil and weather conditions. This project helps farmers and agri-tech platforms make data-driven planting decisions to **maximize yield and sustainability**.

---

## Problem Statement

Farmers often face uncertainty about which crop to grow on their land due to fluctuating environmental conditions. The goal of this project is to build an intelligent system that can recommend the best crop based on input parameters like:
- Nitrogen (N)
- Phosphorus (P)
- Potassium (K)
- Temperature
- Humidity
- pH level
- Rainfall

---

## Dataset

- Source: [Kaggle – Crop Recommendation Dataset](https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset)
- Features:
  - `N`, `P`, `K` — Nutrient levels
  - `temperature`, `humidity` — Weather conditions
  - `ph` — Soil pH value
  - `rainfall` — mm rainfall
- **Target column**: `label` → the recommended crop (e.g., rice, maize, mango, cotton)

---

## Model Details

| Attribute | Value |
|----------|-------|
| **ML Type** | Multi-class classification |
| **Target** | `label` (name of the crop) |
| **Algorithm Used** | Random Forest Classifier |
| **Accuracy** | ~96% on test data |
| **Tools** | Python, Pandas, Scikit-learn, Matplotlib, Seaborn |

---

## 🛠How It Works

1. **Preprocessing**
   - Cleaned and normalized features
   - Encoded the `label` column (for training)

2. **Model Training**
   - Trained a **Random Forest** for high performance and interpretability
   - Evaluated using accuracy, classification report, and confusion matrix

3. **Prediction Example**
```json
Input:
{
  "N": 90,
  "P": 42,
  "K": 43,
  "temperature": 24.5,
  "humidity": 82.3,
  "ph": 6.4,
  "rainfall": 205.0
}
↓
Prediction: "rice"
```
## Results:

