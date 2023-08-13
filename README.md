# AllStateInsurance
This project is among Kaggle's competitions and participants were asked to predict the `loss` variable which stands for the cost of accidents and hence the severity of the insurance claims. In fact, each row in this dataset represents an insurance claim. The main challenge of this dataset is the abundance of features: 116 categorical features (variables that are prefaced with 'cat') and 14 continuous features (variables that are prefaced with 'cont'). To handle these challenges, we performed a wide range of preprocessing techniques. To be more specific, for categorical features, after removing features that were highly correlated to others using the Cramers' V method, we used the following techniques for feature encoding:

- One-hot encoding
- Target encoding

For continuous features, we used the following methods for feature scaling: 

- StandardScaler
- Quantile encoding (based on the uniform distribution)
- Quantile encoding (based on the normal distribution)

For continuous features, we also performed the PCA technique which could not help in boosting model performance.

We built several models on this data and as we expected the XGBoost model returned the best performance. 

The Notebook is designed to be self-contained.
