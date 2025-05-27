# Linear Regression Model for Retail Demand Prediction

## 📈 Project Overview

This project uses a Linear Regression model to predict **product demand** based on retail sales data. The dataset includes a mix of numeric and categorical features such as inventory levels, pricing, discounts, weather conditions, and more.

The primary objective is to forecast product demand to support inventory planning, marketing decisions, and supply chain optimization.

---

## 🧾 Dataset Description

The dataset includes the following columns:

### 🔢 Numeric Features:
- `Inventory Level`
- `Units Sold`
- `Units Ordered`
- `Price`
- `Discount`
- `Competitor Pricing`
- `Demand` (Target)
- `Year`
- `Promotion`

### 🔤 Categorical Features:
- `Store ID`
- `Product ID`
- `Category`
- `Region`
- `Weather Condition`
- `Seasonality`

---

## 🛠️ Steps Performed

1. **Data Preprocessing**:
   - Encoded categorical variables using `OneHotEncoder`.
   - Normalized numerical features (optional depending on model pipeline).
   - Handled missing values and ensured data type consistency.

2. **Model Training**:
   - Used `scikit-learn`’s `LinearRegression`.
   - Split data into training and testing sets (e.g., 80/20 split).
   - Evaluated using metrics like **R²**, **MAE**, and **RMSE**.

3. **Model Saving**:
   - Trained model was saved using `joblib`:
     ```python
     import joblib
     joblib.dump(model, 'model.pkl')
     ```

---

## 📊 Evaluation Metrics

The following metrics were used to assess model performance:
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**

