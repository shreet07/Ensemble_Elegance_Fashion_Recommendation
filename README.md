# Ensemble_Elegance_Fashion_Recommendation
A machine learning project using Stacked Generalization to classify Fashion-MNIST images. Ensembles Random Forest, SVM, KNN, and Decision Trees with a Logistic Regression meta-learner to predict fashion trends. Demonstrates superior accuracy over individual models by combining diverse classifier strengths.

# Ensemble Elegance: Fashion Classification using Stacked Generalization

## 📌 Project Overview
Ensemble Elegance is a Machine Learning project that leverages **Stacked Generalization (Stacking)** to classify images from the Fashion-MNIST dataset. By combining multiple diverse base models (Random Forest, SVM, KNN, Decision Tree), this project demonstrates how ensemble methods can improve predictive performance and model robustness compared to individual classifiers[cite: 13, 14].

[cite_start]This project was completed as a **6th Semester Machine Learning dissertation**, emphasizing both technical implementation and strategic business analysis[cite: 1, 3].

## 📂 Dataset
[cite_start]The project uses the **Fashion-MNIST** dataset, a drop-in replacement for the classic MNIST handwritten digits dataset[cite: 17].
* **Training Set:** 60,000 images
* **Test Set:** 10,000 images
* [cite_start]**Classes:** 10 fashion categories (e.g., T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot)[cite: 18].
* [cite_start]**Format:** 28x28 grayscale images[cite: 17].

## 🛠️ Tech Stack
* **Language:** Python
* [cite_start]**Libraries:** Scikit-learn, NumPy, Pandas, Matplotlib, Seaborn[cite: 20].
* [cite_start]**Base Models:** Random Forest, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), Decision Tree[cite: 25].
* [cite_start]**Meta-Learner:** Logistic Regression[cite: 25].

## 📊 Methodology (Stacked Generalization)
1.  [cite_start]**Data Preprocessing:** Images were flattened and normalized (pixel values scaled to 0-1 range)[cite: 21].
2.  [cite_start]**Base Layer Training:** Four distinct classifiers were trained independently on the training data[cite: 25].
3.  [cite_start]**Stacking:** The predictions (probabilities) from these base models were used as **new features** to train a final **Meta-Learner** (Logistic Regression).
4.  [cite_start]**Final Prediction:** The meta-learner makes the final classification based on the combined insights of the base models.

## 📈 Results & Performance
[cite_start]The Stacking Classifier achieved a final accuracy of **89%**, matching the best individual performer (SVM) while offering potentially better generalization[cite: 35].

| Model | Accuracy |
| :--- | :--- |
| **Decision Tree** | [cite_start]79% [cite: 34] |
| **KNN** | [cite_start]86% [cite: 33] |
| **Random Forest** | [cite_start]88% [cite: 31] |
| **SVM** | [cite_start]89% [cite: 32] |
| **Stacking Classifier (Final)** | [cite_start]**89%** [cite: 35] |

## 🧠 Learning Outcomes
Beyond technical execution, this project encompassed a holistic business approach:
* **Strategic Communication:** Designed an investor-ready pitch deck to present the project's value proposition.
* **Financial Literacy:** Analyzed cash flow statements and developed financial marketing strategies for a theoretical product launch.
* **Professional Branding:** Optimized professional portfolios and resumes to align with industry standards.

## 🚀 Installation & Usage
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/Ensemble-Elegance-Fashion.git](https://github.com/yourusername/Ensemble-Elegance-Fashion.git)
