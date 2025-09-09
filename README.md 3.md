# Task 3: Multimodal ML – Housing Price Prediction Using Images + Tabular Data

## 📌 Objective
The goal of this task is to build a **multimodal machine learning model** that predicts **housing prices** by combining information from **tabular data (structured features)** and **house images (unstructured visual data)**.  
This approach leverages the strengths of both data modalities to improve prediction accuracy.

---

## 🔧 Methodology / Approach
1. **Dataset**
   - **Tabular Data**: Housing sales dataset containing structured features (e.g., number of rooms, area, location).
   - **Image Data**: House images dataset (custom-collected or publicly available).

2. **Image Feature Extraction**
   - Use **Convolutional Neural Networks (CNNs)** (e.g., ResNet, VGG, or custom CNN) to extract high-level features from house images.
   - Apply transfer learning or train a custom CNN depending on dataset size.

3. **Tabular Data Preprocessing**
   - Handle missing values, encode categorical features, and scale numerical features.
   - Ensure features are normalized and compatible with fusion.

4. **Feature Fusion**
   - Concatenate **CNN-extracted image features** with **processed tabular features**.
   - Feed combined features into a fully connected regression model.

5. **Model Training & Evaluation**
   - Train the multimodal model on combined features.
   - Evaluate performance using **Mean Absolute Error (MAE)** and **Root Mean Squared Error (RMSE)**.

---

## 📊 Key Results / Observations
- **Multimodal Advantage**: Combining images with tabular data led to more accurate price predictions compared to using either modality alone.
- **CNN Effectiveness**: Pretrained CNNs (e.g., ResNet) provided robust feature extraction for house images, improving model generalization.
- **Feature Fusion**: Early fusion (concatenating features before regression) worked effectively for this task.
- **Evaluation Metrics**: MAE and RMSE clearly reflected improvements from multimodal learning, showing reduced error rates compared to baseline models.

---

## 🚀 Skills Gained
- Designing **multimodal ML architectures** for real-world regression tasks.
- Applying **Convolutional Neural Networks (CNNs)** for visual feature extraction.
- Implementing **feature fusion** techniques to integrate multiple data sources.
- Building and evaluating regression models with **MAE** and **RMSE** metrics.
