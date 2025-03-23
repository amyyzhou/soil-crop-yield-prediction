# 🌱 Soil Microbiome-Based Crop Yield Prediction

This project explores how the composition of soil bacteria can be used to predict barley crop yields using machine learning. By analyzing microbiome sequencing data and crop yield metadata from Australian farms, the project demonstrates how soil health and microbial diversity impact agricultural productivity.

---

## 📁 Project Structure

- `bacteria_counts_lognorm.csv`  
  Log-normalized bacterial abundance data for each farm's soil sample.

- `sample_metadata.tsv`  
  Metadata for each farm, including the target variable: `crop_yield`.

- `Soil Analysis`  
  Additional soil property data (optional, not yet integrated).

- `main.py` *(or your notebook/script name)*  
  Core script for loading data, training models, and evaluating performance.

---

## 🔍 What the Project Does

1. **Loads and preprocesses** microbiome and crop yield data  
2. **Trains and evaluates** multiple machine learning models:
   - Decision Tree Regressor
   - Linear Regression
   - MLP (Neural Network) Regressor
   - K-Nearest Neighbors Regressor
3. **Computes Relative Squared Error (RSE)** to benchmark against a simple mean-based predictor
4. **Visualizes model performance** with scatter plots and bar charts comparing RSE across models

---

## 📊 Sample Output

Model Comparison (RSE):

| Model           | RSE   |
|----------------|--------|
| MLP Regressor  | 0.265 |
| KNN Regressor  | 0.386 |

![Bar Chart: Model Comparison](#)

---

## 🛠️ Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Install requirements with:

```bash
pip install -r requirements.txt
```

---

## 💡 Future Improvements

- Add ensemble models (Random Forest, Gradient Boosting)
- Integrate soil chemistry/structure data
- Implement cross-validation
- Build a Streamlit or Flask web app for interactive prediction

---

## 🧠 Author
