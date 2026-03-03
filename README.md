# Ensemble_Elegance_Fashion_Recommendation

This project is a deep learning-based recommendation engine designed to provide visually similar fashion suggestions. It utilizes state-of-the-art Convolutional Neural Networks (CNNs) to analyze image features and provide relevant product recommendations from a large dataset of fashion items.

# Ensemble Elegance: Fashion Recommendation System

Ensemble Elegance is a state-of-the-art fashion recommendation engine designed to bridge the gap between "seeing" and "finding", an end-to-end Fashion Recommendation System leveraging Computer Vision and Deep Learning (Convolutional Neural Network). By integrating ResNet50, VGG16, and MobileNetV2 for high-dimensional feature extraction with K-Nearest Neighbors (KNN) for similarity mapping, the system delivers precise, visually-aligned style suggestions from a dataset of 44,000+ fashion items."

## 🚀 Features:

* **Visual Similarity Search:** Recommends items based on visual characteristics like shape, color, and texture.
* **Deep Feature Extraction:** Uses pre-trained models (ResNet50) to transform images into dense vector representations.
* **Content-Based Filtering:** Employs K-Nearest Neighbors (KNN) to find the most similar items in the feature space.
* **Interactive Visualizations:** Displays recommended matches alongside their similarity scores.

## Advanced Version:
The engine supports a "Model Zoo" approach, allowing for comparison between different architectures:

* **ResNet50:** Utilizes deep residual learning for robust feature detection.
* **VGG16:** Known for its precise spatial understanding of image textures.
* **MobileNetV2:** Optimized for high-speed inference without compromising accuracy.

**Workflow:** Images are normalized and passed through the pre-trained layers. The final classification head is removed, and Global Average Pooling is applied to generate a 2048-dimensional feature vector (embedding).

**The Recommendation Engine (KNN):**

* **Algorithm:** K-Nearest Neighbors (KNN).
* **Metric:** Euclidean / Cosine Distance.
* **Process:** Every image in the database is pre-processed into an embedding. When a user uploads a photo, the system calculates the distance between the user’s vector and the database vectors, returning the 'K' closest matches.

## 🛠️ Technologies Used:

* **Language:** Python
* **Deep Learning Framework:** TensorFlow / Keras
* **Computer Vision:** OpenCV, Pillow (PIL), scikit-image
* **Data Analysis:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (StandardScaler, PCA, NearestNeighbors)
* **Visualization:** Matplotlib, Seaborn, Plotly

## 📂 Dataset:

The system is built using a dataset containing over **44,000 fashion images** labeled with metadata such as gender, category, sub-category, and product type.

* **CSV Data:** `styles.csv` containing product attributes.
* **Image Data:** High-resolution images of various fashion products.

## 🏗️ Project Workflow

1. **Exploratory Data Analysis (EDA):** Analyzing product distribution by category, gender, and season using Plotly charts.
2. **Image Preprocessing:** Resizing and normalizing images for model compatibility.
3. **Feature Extraction:** Leveraging a pre-trained **ResNet50** model to extract high-level visual features.
4. **Similarity Search:** Using a `NearestNeighbors` algorithm to calculate the distance between a query image and the database.
5. **Recommendation Engine:** A custom function that takes an image path and returns the top "N" similar products.

## 📊 Visualizations

The project includes several analytical plots:

* **Product Distribution by Season:** A circular plot showing seasonal trends.
* **Top Article Types:** Horizontal bar charts identifying common items like T-shirts, Shirts, and Casual Shoes.
* **Category Flow:** Parallel category diagrams showing the flow between gender, category, and usage.
