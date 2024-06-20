# Housing Price Prediction

## Project Description

The goal of this project is to predict housing prices with high accuracy. We start with extensive data preprocessing and exploratory data analysis to understand the data and its structure. Advanced clustering techniques like t-SNE and UMAP are used to explore the underlying data patterns, followed by linear regression and PCA for feature reduction. We implement Stacking Regression, a robust ensemble method, to enhance model accuracy. The entire process is orchestrated through an end-to-end pipeline using DataBricks clusters.

## Data Collection

Data for this project is collected from publicly available datasets such as the [Kaggle Housing Prices Competition](https://www.kaggle.com/c/house-prices-advanced-regression-techniques). Ensure you have the necessary permissions to use and distribute the data.

## Data Preprocessing

We employ the following steps for data preprocessing:

1. **Handling Missing Values:** Various imputation techniques are used, including mean, median, mode, and predictive modeling, depending on the nature of the missing data.
2. **Categorical Encoding:** Encoding categorical variables using One-Hot Encoding, Label Encoding, or Target Encoding as appropriate.
3. **Feature Scaling:** Standardizing numerical features to a common scale.
4. **Variable Segregation:** Separating numerical, categorical, and continuous variables for tailored preprocessing.

## Exploratory Data Analysis

EDA involves:

1. **Statistical Summaries:** Descriptive statistics for each feature.
2. **Correlation Analysis:** Visualizing correlations between features and the target variable using heatmaps.
3. **Distribution Analysis:** Histogram plots for numerical features.
4. **Boxplots and Scatterplots:** For outlier detection and relationship analysis.

## Feature Engineering

Feature engineering includes:

1. **Creating Derived Features:** New features based on domain knowledge.
2. **Interaction Features:** Combining features to capture interactions.
3. **Polynomial Features:** For capturing non-linear relationships.

## Dimensionality Reduction

Principal Component Analysis (PCA) is used to reduce the dimensionality of the dataset while preserving variance:

- **Variance Explained:** Selecting the number of components based on cumulative variance explained.

## Clustering

Advanced clustering techniques:

1. **t-SNE:** For visualizing high-dimensional data in 2D space.
2. **UMAP:** Used for enhancing clustering and group identification.

## Modeling

Stacking Regression is utilized to combine multiple regression models to improve prediction accuracy:

1. **Base Models:** Linear Regression, Decision Trees, Random Forest.
2. **Meta-Model:** Aggregates predictions from base models.
3. Other models include:
   - **Linear Regression:** For baseline comparisons.

## Evaluation

Model evaluation metrics:

1. **RMSE:** Root Mean Squared Error.
2. **MAE:** Mean Absolute Error.
3. **R² Score:** Coefficient of determination.

Cross-validation techniques are applied for robust evaluation.

## End-to-End Pipeline

An end-to-end pipeline is created using DataBricks clusters, ensuring a scalable and efficient workflow:

1. **Data Ingestion:** Loading data from various sources.
2. **Preprocessing:** Automated data cleaning and preparation.
3. **Model Training:** Orchestration of model training and tuning.
4. **Model Evaluation:** Automated performance evaluation.
5. **Deployment:** Deploying the model for predictions.

## Setup and Installation

### Prerequisites

- **Python 3.8+**
- **DataBricks Account**
- **Git**
- **Libraries:** Install dependencies from `requirements.txt`

### Installation Steps

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/hardeek24/housing-price-prediction.git
    cd housing-price-prediction
    ```

2. **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Setup DataBricks Cluster:**
    1. Create and configure a DataBricks cluster.
    2. Upload and link your project files.

## Future Enhancements

We can apply hard rules for separate clusters and run the models separately. Data can be split between different clusters and model performance can be evaluated for different algorithms and rules. In this way, we can reduce bias, data leakage, and optimize the model to give predictions with maximum accuracy.
