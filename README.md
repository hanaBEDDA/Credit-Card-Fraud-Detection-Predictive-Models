# Credit-Card-Fraud-Detection-Predictive-Models

# Problem statement
The selected project aims to utilize machine learning models for the prediction of fraudulent credit card transactions. Our analysis is based on customer-level data obtained through a collaborative effort between Worldline and the Machine Learning Group. 

The dataset, sourced from [Kaggle](https://www.kaggle.com/), comprises a total of 284,807 transactions, of which 492 are fraudulent. Given the significant class imbalance in the dataset, addressing this imbalance is a necessary preprocessing step before constructing our models.

# Business Problem Overview
You can access the dataset through this provided [link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud). 

The dataset comprises credit card transactions conducted by European cardholders during a two-day period in September 2013. Among the 284,807 transactions, 492 were identified as fraudulent. 
This dataset exhibits a significant class imbalance, with fraudulent transactions making up only 0.172% of the total. Additionally, the dataset has been subjected to Principal Component Analysis (PCA) for confidentiality purposes. With the exception of 'time' and 'amount,' all other features, denoted as V1, V2, V3, up to V28, are derived from PCA. The 'time' feature records the time elapsed in seconds between the first transaction and subsequent ones, while the 'amount' feature represents the transaction amount. The 'class' feature indicates the transaction's class, taking the value 1 for fraud and 0 for non-fraudulent transactions.

# Project Pipeline
The project workflow can be succinctly outlined in four key stages:

1. **Data Understanding:** In this phase, the primary focus is on loading and comprehending the dataset, enabling us to select the relevant features for our final model.

2. **Exploratory Data Analysis (EDA):** Typically, during EDA, we conduct univariate and bivariate analyses of the data and apply feature transformations if necessary. Given that Gaussian variables are utilized in this dataset, Z-scaling is not required. Nevertheless, it's advisable to examine for any data skewness and address it, as it could potentially affect the model-building phase.

3. **Train/Test Split:** After gaining a good understanding of the data, we proceed with the train/test split to assess model performance on unseen data. For validation purposes, we can employ the k-fold cross-validation method, ensuring that the test folds adequately represent the minority class.

4. **Model Building/Hyperparameter Tuning:** This pivotal step involves experimenting with different models and fine-tuning their hyperparameters until we achieve the desired performance on the dataset. Exploring various sampling techniques is also recommended to enhance model effectiveness.

5. **Model Evaluation:** The final stage revolves around evaluating the models using appropriate metrics. It's crucial to note that due to the data's imbalance, accurately identifying fraudulent transactions takes precedence over non-fraudulent ones. Hence, selecting an evaluation metric aligned with this specific business objective is essential.
