# Fundamentals of Machine Learning

Fundamentally, a **machine learning model** is a software application that encapsulates a function to calculate an output value based on one or more input values.

- **Training**: The process of defining the function.
- **Inferencing**: Using the trained function to predict new values.

---

# MACHINE LEARNING

## Supervised Machine Learning

Supervised machine learning uses training data that includes:
- **Features** (input values)
- **Labels** (known output values)

The model learns relationships between features and labels to predict unknown labels in future cases.

---

### Regression

Regression is a supervised machine learning technique where the predicted label is a **numeric value**.

- Regression models predict numeric labels using training data with known feature and label values.

#### Regression Evaluation Metrics

- **Mean Squared Error (MSE)**  
  Measures the average of squared differences between predicted and actual values.

- **Root Mean Squared Error (RMSE)**  
  The square root of MSE, providing error in the same unit as the label.

- **Coefficient of Determination (R-Squared)**  
  Measures how much of the variance in the validation data is explained by the model.

#### Iterative Training
Regression models are trained iteratively to minimize error and improve accuracy.

---

### Classification

Classification is supervised machine learning where the label represents a **category or class**.

---

#### Binary Classification (Sigmoid Function)

- Predicts one of two mutually exclusive outcomes (true/false, positive/negative).
- Logistic regression is used for classification, not regression.
- Uses an S-shaped (sigmoid) function producing values between **0 and 1**.

##### Confusion Matrix Components

- ŷ = 0 and y = 0 → **True Negative (TN)**
- ŷ = 1 and y = 0 → **False Positive (FP)**
- ŷ = 0 and y = 1 → **False Negative (FN)**
- ŷ = 1 and y = 1 → **True Positive (TP)**

##### Binary Classification Evaluation Metrics

- **Accuracy**  
  (TN + TP) ÷ (TN + FN + FP + TP)

- **Recall (True Positive Rate)**  
  TP ÷ (TP + FN)

- **Precision**  
  TP ÷ (TP + FP)

- **F1-Score**  
  (2 × Precision × Recall) ÷ (Precision + Recall)

- **Area Under the Curve (AUC)**  
  - True Positive Rate (TPR) = Recall  
  - False Positive Rate (FPR) = FP ÷ (FP + TN)

---

#### Multiclass Classification

- Predicts one label from multiple possible classes.
- Uses the same train, validate, and evaluate process as other supervised models.

##### One-vs-Rest (OvR)

- Trains one binary classifier per class.
- Each classifier predicts the probability of belonging to its class vs all others.

##### Multinomial Algorithms

- Uses a single model returning a probability distribution across all classes.
- Output probabilities sum to **1.0**.

##### Multiclass Evaluation

- Binary metrics can be calculated per class.
- Aggregate metrics can evaluate overall performance.

---

## Unsupervised Machine Learning

Unsupervised learning uses **feature-only data** with no known labels.
The model discovers patterns and relationships within the data.

---

### Clustering

- Groups observations based on similarity of features.
- Labels are assigned by the algorithm itself.
- Common example: **K-Means**

#### Clustering Evaluation Metrics

- **Average distance to cluster center**
- **Average distance to other cluster centers**
- **Maximum distance to cluster center**
- **Silhouette score**  
  Value between **-1 and 1** (closer to 1 = better separation)

---

# DEEP LEARNING

Deep learning is an advanced form of machine learning that attempts to emulate human brain learning.

- Uses **artificial neural networks**
- Simulates biological neuron behavior using mathematical functions

---

# Azure Machine Learning

Azure Machine Learning is a cloud service for building and managing ML models.

Capabilities include:
- Data exploration and preparation
- Model training and evaluation
- Model registration and management
- Model deployment
- Responsible AI implementation

---

=========================================================================

## Algorithm Categories

- **Classification**: Predicts predefined categories
- **Regression**: Predicts numeric values
- **Clustering**: Groups similar data points without labels

### Learning Types

- **Supervised Learning**: Regression, Classification
- **Unsupervised Learning**: Clustering

> **Featurization is NOT a learning type**  
> It includes feature engineering, scaling, and normalization.

---

=========================================================================

### Example Question

**Predicting diabetes probability using age and body fat percentage**

Correct answer:
- **Two features and one label**

Explanation:
- Features: age, body fat percentage
- Label: probability of developing diabetes

---

=========================================================================

## Regression Notes

- Features generate predictions for labels.
- Training and validation datasets both include known labels.
- Multiple linear regression uses multiple independent features.
- Regression uses historical labeled data (supervised learning).

---

## Automated ML Notes

- Supports classification, regression, and time-series forecasting.
- Does NOT support clustering.
- Inferencing pipelines are not models.

---

=========================================================================

### Azure ML Designer – Data Transformation Modules

Correct answers:
- **Clean Missing Data**
- **Normalize Data**
- **Select Columns in Dataset**

Incorrect:
- Evaluate Model (evaluation)
- Train Clustering (training)

---

=========================================================================

## Azure ML Workflow

- Create **Workspace**
- Access **Machine Learning Studio**
- Create **Pipeline**
- Add **Dataset**
- Add **Training Modules**
- Train model
- Deploy to **Endpoint**
- Use **Compute Clusters** for training
- Deploy using **ACI or AKS**

Notes:
- Endpoints must be deployed before testing.
- Automated ML handles validation automatically.

---

## Additional Concepts

- Linear regression: single feature
- Multiple linear regression: multiple features
- Logistic regression: classification
- Hierarchical clustering: unsupervised grouping
- Validation dataset evaluates trained model performance
- Feature engineering is part of data preparation
- K-Means is an unsupervised clustering algorithm
