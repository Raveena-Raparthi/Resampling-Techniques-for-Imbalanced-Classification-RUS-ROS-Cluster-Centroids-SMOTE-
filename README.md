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
  # 4.1 Data Preprocessing
  Cleaned the dataset
  Scaled the features
  Split the data into training and testing sets

  # 4.2 Resampling Techniques
  Random Undersampling : Removing samples from the majority class in order to match the minority class is known as random     undersampling.
  Random Oversampling : To balance classes, random oversampling duplicates samples from minority classes.
  Cluster Centroids: By substituting them with cluster centers, the majority class is reduced.
  SMOTE: Uses feature similarities to generate synthetic (new) samples for the minority class.

  # 4.3 Model Used
  Logistic Regression was used because it is simple, fast, and easy to interpret.

  # 4.4 Evaluation Metrics
    Accuracy
    Precision
    Recall
    F1-score
    AUC-ROC

  # 4.5 Class Distribution Before & After Resampling
    #Random Undersampling
      Before:
        Class 0: 573,518
        Class 1: 21,694
      After:
        Class 0: 21,694
        Class 1: 21,694
    
    #Random Oversampling
      Before:
        Class 0: 573,518
        Class 1: 21,694
      After:
        Class 0: 573,518
        Class 1: 573,518

    #Cluster Centroids
      Before:
        Class 0: 573,518
        Class 1: 21,694
      After:
        Class 0: 20
        Class 1: 21,694

    #SMOTE
      Before:
        Class 0: 573,518
        Class 1: 21,694
      After:
        Class 0: 458,814
        Class 1: 458,814
        
# 5.Model Performance
      F1 Score (0.09) and AUC-ROC (0.57) indicate initial model performance and the potential gains achievable through resampling.

     Class 0 (Majority class): Precision = 0.97, Recall = 0.59, F1-score = 0.74
     → The model predicts most majority-class samples correctly.

     Class 1 (Minority class): Precision = 0.05, Recall = 0.55, F1-score = 0.09
     → The model struggles to identify minority-class samples, showing the need for resampling to improve performance.

# 6.Observations
  On unbalanced data, the model does poorly.
  Minority class prediction is enhanced by oversampling and SMOTE.
  Undersampling reduces accuracy and eliminates a large amount of data.
  Because SMOTE generates new synthetic samples, it typically produces the most balanced results.

# 7.Conclusion
 
  Imbalanced data can reduce a model’s ability to predict the minority class. Resampling techniques help by balancing the    dataset and improving performance. Among the methods tested, SMOTE gave the best results by creating a balanced dataset    without losing information. This project highlights the importance of handling imbalance for accurate and fair models.


# 8.Technologies Used
    Python
    Pandas
    NumPy
    Scikit-learn
    Matplotlib4.9 


    

  
