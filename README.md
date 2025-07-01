

# 🚕 Predicting Generous Tips in New York City Taxis

**A predictive model to anticipate whether a passenger will leave a tip ≥20%, using data from the NYC Taxi and Limousine Commission (TLC NYC).**

![image](https://github.com/user-attachments/assets/9c20f2d5-3b05-4188-a2a7-bae1770fb8c5)

## 📌 Project Objective

To implement Machine Learning models capable of predicting—with high accuracy—a passenger’s likelihood of leaving a generous tip *before* the ride begins, supporting improved service strategies and driver incentives.

## 🗃️ Data Used

- TLC NYC dataset  
- Over 22,000 historical ride records  
- Features: total fare, distance, payment type, tolls, date & time  
- Target variable: `generous` → 1 if tip was ≥20%

## 🤖 Models Built

| Model              | Accuracy | Recall (Generous) | AUC   |
|-------------------|----------|-------------------|-------|
| Random Forest     | 78%      | 86%               | 0.83  |
| XGBoost           | 81%      | 100%              | 0.84  |
| ✅ Best Model       | XGBoost with perfect recall and strong discrimination power |

📌 *When removing the variable `video_view_count` (if present), the model retains AUC 1.00 → no clear signs of overfitting.*

## 🔍 Key Findings

- **Payment type** is the most decisive predictor  
- **High fares and long trips** correlate with generous tips  
- **XGBoost** detects all positive cases, though with a few more false positives

## 🧩 Repository Structure

📁 data/           → Anonymized trip datasets  
📁 notebooks/      → Model training and evaluation  
📁 docs/           → Final report (PDF)  
📄 README.md       → This document

## 🚀 Next Steps

- Integrate the model into the TLC NYC mobile app  
- Add external features (e.g., weather, traffic)  
- Automate driver recommendation system

## 👤 Author

Developed by **Juan**, a data analyst passionate about real-world projects that elevate customer experience.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

