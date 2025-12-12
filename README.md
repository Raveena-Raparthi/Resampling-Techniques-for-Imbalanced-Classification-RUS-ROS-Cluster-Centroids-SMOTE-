# Resampling-Techniques-for-Imbalanced-Classification-RUS-ROS-Cluster-Centroids-SMOTE-

# 1.Project Overview
The goal of this project is to use resampling methods like oversampling, undersampling, Cluster Centroids, and SMOTE to correct imbalanced datasets.  To compare how each approach enhances minority class prediction, a Logistic Regression model is trained.

# 2.Data from the Dataset
  It is a dataset for binary classification.
  There are numerous samples in class 0.
  There aren't many samples in Class 1.
  The model is unable to effectively learn minority patterns as a result of this imbalance.
  
# 3.Problem Statement
When the number of samples in both classes is comparable, machine learning models perform best.  However, the model primarily learns from the majority class and ignores the minority class when the data is unbalanced.  As a result, even though the overall accuracy appears to be high, it predicts the minority class poorly.  In order to balance the data and assess how they enhance the model's learning and performance, this project employs a variety of resampling techniques.

# 4.Methods Used
  **4.1 Data Preprocessing**
  Cleaned the dataset
  Scaled the features
  Split the data into training and testing sets

  **4.2 Resampling Techniques**
  Random Undersampling : Removing samples from the majority class in order to match the minority class is known as random     undersampling.
  Random Oversampling : To balance classes, random oversampling duplicates samples from minority classes.
  Cluster Centroids: By substituting them with cluster centers, the majority class is reduced.
  SMOTE: Uses feature similarities to generate synthetic (new) samples for the minority class.

  **4.3 Model Used**
  Logistic Regression was used because it is simple, fast, and easy to interpret.

  **4.4 Evaluation Metrics**
    Accuracy
    Precision
    Recall
    F1-score
    AUC-ROC

  **4.5.Resampling Techniques Used**
      Random Undersampling,
      Random Oversampling,
      Cluster Centroids,
      SMOTE (Synthetic Minority Oversampling Technique)
  
# 5.Model Performance
**SMOTE**
     F1 Score (0.09) and AUC-ROC (0.57) show that the model is learning but still has room to improve, and SMOTE helps in balancing the dataset for better minority-class recognition.

Class 0 (Majority class): Precision = 0.97, Recall = 0.59, F1-score = 0.74
→ The model performs well on the majority class.

Class 1 (Minority class): Precision = 0.05, Recall = 0.55, F1-score = 0.09
→ SMOTE improves recall, but overall performance on the minority class still needs enhancement.

**Cluste Centroids**
    F1 Score (0.086) and AUC-ROC (0.56) indicate slightly reduced performance compared to SMOTE, mainly due to loss of information from heavy undersampling.

Class 0 (Majority class): Precision = 0.97, Recall = 0.54, F1-score = 0.70
→ Undersampling reduces recall, affecting majority-class predictions.

Class 1 (Minority class): Precision = 0.05, Recall = 0.59, F1-score = 0.09
→ Recall improves, but overall minority-class performance remains low due to limited training samples.

# 6.Observations
  The model performs well on the majority class but struggles heavily with the minority class due to imbalance. Accuracy appears high, but the F1 and AUROC scores show that the model is biased. This clearly indicates the need for resampling.
  
# 7.Conclusion
   Training on an unbalanced dataset leads to poor minority-class detection and unreliable performance. These results show that balancing the data is essential for improving fairness and building a more accurate model.

# 8.Technologies Used
    Python
    Pandas
    NumPy
    Scikit-learn
    Matplotlib4.9 


    

  
