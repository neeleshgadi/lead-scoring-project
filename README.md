🧠 Lead Scoring System – Machine Learning Powered
🚀 What is This?
A machine learning-based Lead Scoring Model that ranks users from Low → Medium → High based on their likelihood to convert (place an order) on a food ordering website. It helps prioritize leads so businesses can focus on high-value customers and boost conversion rates.

🏗️ How It Works (Noob-Friendly 🧃)
1. Collect Data:
Behavioral features like:

✅ Session Time

✅ Order Frequency

✅ Cart Abandonment

✅ Total Spend

2. Clean & Prepare:
Fill missing values

Encode categories with LabelEncoder

Scale features for model performance

3. Train Model:
Use Random Forest Classifier to detect conversion patterns

4. Predict & Score:
Predict probability of conversion

Calculate Lead Score (0–100) using model + feature importance

Classify leads:

High (70+)

Medium (40–70)

Low (<40)

5. Save & Export:
Save results to CSV

Save trained model and encoders with joblib

🎯 Example Output

User ID	Order Freq	Session Time	Lead Score	Lead Quality
123	3/week	5 mins	88	High
456	1/week	2 mins	45	Medium
789	None	1 min	25	Low
📌 Top Features Influencing Score
🔥 Order Frequency (most impact)

😬 Cart Abandonment Rate

⏳ Session Duration

💰 Total Spend

📱 Device Type

💾 Files in Repo
lead_scoring_model.pkl: Trained model

scaler.pkl, label_encoder.pkl: Preprocessing tools

lead_scoring_results.csv: Final lead scores and labels

lead_scoring.ipynb: Full source code

lead_scoring_synthetic.csv : Dataset

✅ Why Use This?
Tracks real customer behavior

Helps marketing teams act fast

Improves ROI and reduces time wasted on low-quality leads
