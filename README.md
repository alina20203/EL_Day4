# ElevateLabs_Task 4

## **Taks 4**:  Classification with Logistic Regression

Logistic Regression is a machine learning algorithm used for binary classification tasks. Unlike linear regression, which predicts continuous outcomes, logistic regression predicts the probability of class membership (e.g., yes/no, 0/1). It uses the sigmoid function to map any real-valued number into a range between 0 and 1. Based on this probability, predictions are made using a classification threshold (typically 0.5).

## **Dataset**

diabetes.csv

## **Tools**

- Python<br>
- Numpy<br>
- Pandas<br>
- Numpy<br>
- Seaborn<br>
- Scikit-learn<br>
- Jupyter Notebook<br>

# **Tasks Performed in the dataset**

## 1. Import and preprocess the dataset

The first step involves importing the dataset for initial exploration. Any missing or inconsistent data entries are handled appropriately, Categorical variables are encoded into numerical values,etc to ensure a clean and reliable dataset for model building.

## 2. Train/Test Split and Feature Standardization

We split the dataset into a training set (80%) and a testing set (20%) using train_test_split. Since logistic regression is sensitive to feature scale, we standardize the data using StandardScaler to bring all feature values to a similar scale.

## 3. Fit the Logistic Regression Model

Using Scikit-learn’s LogisticRegression class, we train the model on the scaled training data. The model learns weights for each feature and uses them to predict probabilities for the positive class.

## 4. Model Evaluation
We evaluate the trained model using multiple metrics:
- Confusion Matrix: Shows true/false positives and negatives.
- ROC-AUC Curve: Plots true positive rate vs false positive rate, indicating model’s ability to distinguish between classes.

## 5.Sigmoid Function

The model predicts a probability score, which is passed through a sigmoid function.We can adjust the decision threshold (default is 0.5) to optimize for different performance goals. 
