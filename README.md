# wine_quality_prediction
Predicting Wine Quality Using ML

# Wine Quality Prediction using Machine Learning

This project aims to predict the quality of wine using various machine learning techniques. The dataset includes several chemical properties of the wine, and the goal is to classify the quality of the wine as either good or bad.

## Dataset

The dataset can be found on Kaggle: [Red Wine Quality](https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009).

The dataset consists of the following columns with 1599 rows:

- `fixed acidity`: Fixed acidity of the wine
- `volatile acidity`: Volatile acidity of the wine
- `citric acid`: Citric acid content of the wine
- `residual sugar`: Residual sugar content in the wine
- `chlorides`: Chloride content in the wine
- `free sulfur dioxide`: Free sulfur dioxide content in the wine
- `total sulfur dioxide`: Total sulfur dioxide content in the wine
- `density`: Density of the wine
- `pH`: pH level of the wine
- `sulphates`: Sulphate content in the wine
- `alcohol`: Alcohol content in the wine
- `quality`: Quality of the wine (integer values)

## Data Preprocessing

1. **Data Visualization**: 
   - Used various plots (countplot, barplot, histplot) to study the relationships between the columns.
   - Used a heatmap and `corr()` function to visualize and understand the correlations between features.

2. **Encoding Quality Column**: 
   - Converted the `quality` column to binary values (1 if quality > 6, else 0) using the `apply()` function.

3. **Splitting Data**: 
   - Performed train-test split to create training and testing datasets.

4. **Scaling Data**: 
   - Used `StandardScaler` to scale the features.

## Models Used

1. **Logistic Regression**: 
   - Used for training the primary model.

2. **Support Vector Classifier (SVC)**: 
   - Used for comparison with Logistic Regression.

3. **Random Forest Classifier**: 
   - Used for comparison with Logistic Regression and SVC.

## Evaluation

The models were evaluated using the following metrics:

- **Confusion Matrix**: To visualize the performance of the classification models.
- **Accuracy Score**: To measure the percentage of correctly predicted instances.
- **Classification Report**: To provide precision, recall, f1-score, and support for each class.

### Results

- **Logistic Regression**: Achieved an accuracy of 88.3%.
- **Support Vector Classifier**: Achieved an accuracy of 86.4%.
- **Random Forest Classifier**: Achieved an accuracy of 93.3%.



## How to Use

### Cloning the Repository

To clone the repository, use the following command:

```bash
git clone https://github.com/riitk/wine_quality_prediction.git
cd wine-quality-prediction
