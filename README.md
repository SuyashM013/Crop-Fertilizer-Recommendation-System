# Crop Fertilizer Recommendation System

## 📌 Overview
This project is a **Crop and Fertilizer Recommendation System** that suggests the best crop and suitable fertilizer based on soil nutrients (NPK), environmental factors (temperature, humidity, pH, rainfall), and soil type. The system is implemented using **Python, Jupyter Notebook, Pandas and Scikit-Learn**.

## 🚀 Features
- Predicts the most suitable **crop** for given soil and environmental conditions.
- Recommends an appropriate **fertilizer** for the predicted crop.
- Uses **RandomForestClassifier** for crop prediction.
- Reads **custom datasets** for accurate recommendations.

## 📂 Datasets
This project uses **two datasets**:
1. **Crop_recommendation.csv** - Contains details about soil nutrients and crop suitability.
2. **Fertilizer Prediction.csv** - Maps crops to their ideal fertilizers.

## 🛠 Installation
Follow these steps to set up the project:

### 1️⃣ Install Dependencies
```bash
pip install pandas numpy scikit-learn
```

### 2️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/crop-fertilizer-recommendation.git
cd crop-fertilizer-recommendation
```

### 3️⃣ Open Jupyter Notebook
```bash
OPEN Recommendation.ipynb 
```
Then, run the provided notebook file.

## 📜 Usage
### **Example Prediction**
```python
predicted_crop, recommended_fertilizer = recommend_crop_fertilizer(90, 42, 43, 20.8, 82.0, 6.5, 202.9, 'Sandy')
print(f"Recommended Crop: {predicted_crop}, Recommended Fertilizer: {recommended_fertilizer}")
```
### **Expected Output**
```bash
Recommended Crop: Rice, Recommended Fertilizer: Urea
```

## 🏗 How It Works
1. **Train Model** → Uses `RandomForestClassifier` on `Crop_recommendation.csv`.
2. **Predict Crop** → Based on NPK, temperature, humidity, pH, and rainfall.
3. **Match Fertilizer** → Looks up the best fertilizer from `Fertilizer Prediction.csv`.
4. **Return Recommendation** → Outputs the crop and fertilizer.

## 🔧 Potential Improvements
- Enhance the model with **hyperparameter tuning**.
- Add more **environmental parameters** like altitude, sunlight, etc.
- Deploy as a **web application** using Flask or FastAPI.

