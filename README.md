# Ensemble-Techniques-Ben-Hardy
This notebook utilizes a number of ensemble methods (bagging and boosting) for a supervised learning classification problem. In this case a (fictional) tourism agency wishes to predict which customer is more likely to purchase a newly introduced travel package. The previous marketing strategy was to market to all customers. By classifying customers more suited to the new travel package, the company hopes to reduce marketing costs and increase customer uptake.

The notebook (Tourism_Project) was generated for the fourth project of the Post Graduate Program in Artificial Intelligence and Machine Learning: Business Applications from the McCombs School of Business at The University of Texas. The data was provided in a .csv file.

The notebook has an extended EDA section. The data are synthetic and fairly clean given that they were provided for a school project. That said there were some nulls and outliers that needed to be addressed. I used relationships between the variables to fill null values in the case of continuous variables. I used median values per category for other variables. Categorical variables were then encoded and modelling begins.

Models used: 
From sklearn
Decision Tree, BaggingClassifier, RandomForestClassifier, AdaBoostClassifier, GradientBoostingClassifier
I also used XGBoost and spent some time trying to optimize it, given that it gave the best performance but was initially overfitting the training data. The best model that was not overfitting was an AdaBoostClassifier model.

Hyperparameters were tuned using GrisSearchCV and then, to some extent, by trial and error.

While this project was done as part of a school project. I believe it indicates the quality of work that I’m capable of in real-world applications. I was the top student in my cohort with a final course weighted average of 99.39%. Finally, at the time I didn't have any concept of "data leakage", so I'm just using a train and test set. Nowdays I would split the data into train, validation and test.
