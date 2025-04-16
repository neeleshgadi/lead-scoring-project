# Lead Scoring System – Machine Learning Powered 🚀

## Overview
A machine learning-based lead scoring model designed to rank users from **Low → Medium → High** based on their likelihood to convert (place an order) on a food ordering website. The system helps businesses prioritize high-value customers and boost conversion rates.

## How It Works 🏗️
1. **Data Collection**: Collect behavioral features such as:
   - **Session Time**
   - **Order Frequency**
   - **Cart Abandonment**
   - **Total Spend**

2. **Data Preprocessing**:
   - Fill missing values.
   - Encode categorical features using `LabelEncoder`.
   - Scale numerical features for optimal model performance.

3. **Model Training**:
   - Use **Random Forest Classifier** to detect conversion patterns.

4. **Prediction & Lead Scoring**:
   - Predict the likelihood of conversion and calculate the lead score (0–100).
   - Classify leads into:
     - **High** (70+)
     - **Medium** (40–70)
     - **Low** (<40)

5. **Save & Export**:
   - Save results to a **CSV** file.
   - Save the trained model and preprocessing tools using **Joblib**.

---

## Example Output 🎯

| User ID | Order Frequency | Session Time | Lead Score | Lead Quality |
|---------|-----------------|--------------|------------|--------------|
| 123     | 3/week          | 5 mins       | 88         | High         |
| 456     | 1/week          | 2 mins       | 45         | Medium       |
| 789     | None            | 1 min        | 25         | Low          |

---

## Key Features Influencing Score 🔥

- **Order Frequency** (most impact)
- **Cart Abandonment Rate**
- **Session Duration**
- **Total Spend**
- **Device Type**

---

## Files in the Repository 📂

- **`lead_scoring_model.pkl`**: Trained machine learning model.
- **`scaler.pkl`**: Feature scaling tool used during training.
- **`label_encoder.pkl`**: Label encoder for categorical data.
- **`lead_scoring_results.csv`**: Final lead scores and classifications.
- **`lead_scoring.ipynb`**: Full source code for the project.
- **`lead_scoring_synthetic.csv`**: A synthetic dataset for training the model.

---

## How to Use 📋

1. **Clone this Repository**:
   ```bash
   git clone https://github.com/your-username/lead-scoring-system.git
   cd lead-scoring-system
