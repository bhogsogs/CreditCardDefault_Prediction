# Credit Card Default Prediction

Creating a Credit Card Default Predictor for FAIR-AI at Enigma, the Machine Learning Event of CodeFest hosted by the CSE Department of IIT (BHU) Varanasi, was an exciting and challenging endeavor. Leveraging advanced Machine Learning and Data Science techniques, I embarked on a journey to develop a robust predictive model that could accurately forecast credit card defaults while ensuring fairness and reliability in its predictions.

The first critical step in this project was data preprocessing. Raw data often contains inconsistencies, missing values, and imbalances that can skew model performance. To mitigate these issues, I meticulously cleaned and transformed the dataset. This involved handling missing data, encoding categorical variables, and scaling numerical features to prepare the data for modeling.

One of the significant challenges I encountered was addressing the gender imbalance present in the dataset. To ensure fairness in model predictions and avoid biases, I employed Synthetic Minority Over-sampling Technique (SMOTE). SMOTE effectively generated synthetic samples of the minority class (in this case, defaulted credit cards) to balance the dataset. By doing so, I aimed to improve the model's ability to generalize and predict accurately across all demographic groups.

For the modeling phase, I opted to use CatBoost, a powerful gradient boosting library known for its robustness and ability to handle categorical features seamlessly. CatBoost is particularly advantageous in scenarios where data includes categorical variables with a large number of levels, as it incorporates them directly into the model without requiring extensive preprocessing.

Achieving optimal model performance required efficient hyperparameter tuning. To expedite this process, I employed Optuna, a hyperparameter optimization framework that automates the search for the best hyperparameters. Optuna utilizes sophisticated algorithms to efficiently explore the hyperparameter space and identify combinations that yield the highest model accuracy. Through iterative trials and evaluations, I fine-tuned the model parameters to maximize predictive performance while ensuring computational efficiency.

# Results

The best performing model was able to secure a best score of 0.52595(out of 1), where the evaluation metric was a combination of the F1 Score and the Demographic Parity Ratio.

(Kaggle Competition link - [link](https://www.kaggle.com/competitions/fair-ai/data))
