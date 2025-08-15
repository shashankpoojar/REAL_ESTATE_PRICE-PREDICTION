# 🏠 Real Estate Price Prediction – Bangalore Housing Market

## 📌 Overview
This project predicts real estate prices in Bangalore using **end-to-end data science techniques** — from raw data cleaning to model deployment.

## 🎯 Objectives
- Clean and preprocess messy real estate data.
- Engineer meaningful features to improve model performance.
- Compare machine learning models and select the best-performing one.
- Prepare the model for deployment with supporting files.

## 📊 Dataset
[Download Dataset](YOUR_DATASET_LINK_HERE)

## 🛠 Data Preprocessing
- Handled missing values and standardized data formats.
- Grouped rare locations into 'other' category.
- Removed outliers based on sqft/bedroom ratios and price-per-sqft.

## ⚙️ Feature Engineering
- Created `price_per_sqft` metric.
- One-Hot Encoding for `location`.
- Selected top features via correlation and covariance analysis.

## 🤖 Model Building
Compared Linear Regression, Lasso, and Decision Tree models using GridSearchCV and Cross-Validation.  
**Best Model:** Linear Regression (92% accuracy).

## 📈 Results
Example Predictions:
```python
predict_price('Indira Nagar', 1000, 3, 3) → ₹93.86 Lakhs  
predict_price('Whitefield', 1000, 5, 5) → ₹65.37 Lakhs
```

## 📸 Visualizations
![Correlation Heatmap](images/correlation_heatmap.png)  
![Price per Sqft Distribution](images/price_per_sqft_dist.png)  
![Scatterplot Outliers](images/scatterplot_outliers.png)  
![Boxplots](images/boxplots.png)  

## 📂 Tech Stack
- Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## 🚀 How to Run
```bash
git clone https://github.com/YOUR_USERNAME/real-estate-price-prediction.git
cd real-estate-price-prediction
pip install -r requirements.txt
jupyter notebook REAL_ESTATE_PRICE_PREDICTION.ipynb
```

## 📜 License
This project is licensed under the MIT License.
