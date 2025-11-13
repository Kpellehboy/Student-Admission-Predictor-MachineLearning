# 🎓 Student Admission Count Predictor (Random Forest Regression)

## 🚀 Project Overview

This project implements an **Ensemble Learning** model, the **Random Forest Regressor**, to predict the **number of students accepted for admission** based on historical entrance data.

**Why Random Forest?** It's a powerful algorithm that handles **non-linear relationships** and is resistant to outliers, making it an excellent choice for real-world predictive tasks like admissions forecasting. The goal is to provide accurate, actionable predictions for resource planning.

### **Key Artifacts**
* `Admission_Prediction_Model.ipynb`: The Jupyter Notebook containing the full code pipeline.

## 🛠️ Tools and Libraries Used

| Category | Tool/Library | Purpose |
| :--- | :--- | :--- |
| **Data Handling** | **Pandas** | Loading and preparing the data (DataFrame creation and quality checks). |
| **Numerical Operations** | **NumPy** | Fundamental numerical computing and formatting the final integer predictions. |
| **Machine Learning** | **Scikit-learn** (`sklearn`) | Core ML library for splitting data, training the model, and evaluation metrics. |
| **Visualization** | **Matplotlib** / **Seaborn** | Creating the charts to visually assess model performance (Actual vs. Predicted plot). |
| **Algorithm** | `sklearn.ensemble.RandomForestRegressor` | The **Ensemble Model** used for training, providing high predictive power. |

## ⚙️ Methodology: The Advanced Pipeline

1.  **Data Preparation:** Defined Features ($X$) and Target ($y$), ensuring data quality.
2.  **Data Splitting:** Used `train_test_split` (80/20) to create dedicated Training and Testing sets.
3.  **Model Training:** Trained the **Random Forest Regressor**. This model uses 100+ decision trees to learn complex patterns and averages their results for a robust prediction.
4.  **Evaluation:** Measured accuracy on unseen data using metrics like **$R^2$ Score** (variance explained) and **Mean Absolute Error (MAE)** (average prediction error in student count).
5.  **Prediction:** Used the highly accurate model to generate a final forecast for a hypothetical enrollment period.


## Plot
![WhatsApp Image 2025-11-13 at 18 36 57_c5f42c1c](https://github.com/user-attachments/assets/3d3828d9-9c12-4d5e-8aa6-c5438c2a8b51)



## Predict New Applicants chances(low chance) The predicted chance of admit is: 0.4855 = 48.55%
![WhatsApp Image 2025-11-13 at 18 39 25_d737f334](https://github.com/user-attachments/assets/4813c090-1d44-4ea1-9dcb-f1ed04add24c)



## Predict New Applicants chances(high chance) The predicted chance of admit is: 0.8872 = 88.72%
![WhatsApp Image 2025-11-13 at 18 41 13_9eeb4cd3](https://github.com/user-attachments/assets/9c0c8eb3-2175-42bd-9dca-cda6b8557ba2)


## 🚀 Next Steps and Future Improvements

* **Hyperparameter Tuning:** Use **Grid Search** or **Randomized Search** to find the optimal settings for the Random Forest (e.g., number of trees, max depth) to squeeze out maximum accuracy.
* **Data Scaling:** While Random Forest is less sensitive, applying `StandardScaler` to features can still be tested as a potential performance boost.
* **Feature Importance:** Extract the built-in feature importance from the Random Forest model to see which input factors (e.g., entrance score vs. applicant count) contributed most to the prediction.


