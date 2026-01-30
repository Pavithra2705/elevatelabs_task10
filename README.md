Project Overview

This project implements a K-Nearest Neighbors (KNN) classifier to recognize handwritten digits using the Sklearn Digits dataset. The goal is to understand distance-based classification, feature scaling, K tuning, and model evaluation.

📂 Dataset

Source: Sklearn Digits Dataset (load_digits())

Samples: 1797 images

Image Size: 8 × 8 pixels

Classes: Digits (0–9)

🛠 Tools & Libraries Used

Python

Scikit-learn

NumPy

Matplotlib

🚀 Steps Performed
1️⃣ Data Loading

Loaded the digits dataset and examined feature and label shapes.

2️⃣ Data Visualization

Displayed sample images to confirm correct digit-label mapping.

3️⃣ Train-Test Split

Split dataset into:

80% Training

20% Testing

4️⃣ Feature Scaling

Applied StandardScaler to normalize features since KNN uses distance metrics.

5️⃣ Model Training

Trained KNN classifier with multiple values of K:

K = 3

K = 5

K = 7

K = 9

6️⃣ Model Evaluation

Compared accuracy for different K values

Selected best K based on highest accuracy

7️⃣ Confusion Matrix

Generated confusion matrix to analyze misclassifications.

8️⃣ Predictions

Displayed test images with predicted labels.

📊 Results

Best Accuracy Achieved: ~98% (may vary slightly)

Model performs well in recognizing handwritten digits

Minor confusion observed between visually similar digits

📈 Accuracy vs K Graph

Shows how model performance varies with different K values and helps in selecting the optimal K.

🔍 Confusion Matrix Insights

Most digits correctly classified

Some errors between similar shapes (e.g., 3 & 5, 8 & 9)

🎯 Key Learnings

✔ KNN is a distance-based classifier
✔ Feature scaling is critical for performance
✔ Optimal K improves accuracy
✔ Confusion matrix helps understand errors

💡 Interview Questions & Answers
❓ What is K in KNN?

K represents the number of nearest neighbors used to classify a new data point.

❓ Why is scaling required for KNN?

Because KNN uses distance metrics, unscaled features may dominate and reduce accuracy.

❓ What is Euclidean Distance?

The straight-line distance between two points:

d = √Σ(x1 - x2)²

❓ What happens if K is too low?

Sensitive to noise

Overfitting

High variance

❓ Limitations of KNN

Slow for large datasets

Memory intensive

Sensitive to noise

Affected by feature scaling

📁 Repository Contents

knn_digits.ipynb → Jupyter Notebook

README.md → Project documentation

Screenshots of results (plots & confusion matrix)

✅ Conclusion

The KNN classifier effectively recognizes handwritten digits with high accuracy. Proper feature scaling and K tuning significantly improve model performance.
