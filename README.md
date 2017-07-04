This project explores the hinge data and provides likelihood estimations of a player liking a subject.
The code is organized into 3 directories:
- Exploration
- Experiments
- Models

Exploration is where the initial data analysis is performed. A couple of features are added as part of the exploration. In addition, we perform smoothing on the age distribution.
Experiments contains code for building a logistic regression model and xgboost classifier.
Models is where all the models are saved.


- What are some of the most important features, and why did you choose the model you did?
Used Logistic Regression as the baseline model. It is the most simple & elegant first model that gives good performance. Performed grid search cross-validation with L1 & L2 penalty. Also, we used PCA and SVD for finding the features that provide the maximum variance in a particular dimension.
- Why did you choose the evaluation metrics that you did? For our use case, which should be considered most heavily in making business decisions? 
Used F1 weighted for scoring since there is an imbalance in the dataset. Can use F1 weighted or Precision Recall curve to evaluate the performance.
- Given this same dataset and more time, what additional ideas would you try out?
Matrix Factoring to find latent vectors for different players and subjects. Use the latent vectors in addition to the features and feed it into Feedforward Neural Network.
- Make a recommendation for next steps -- what other data sources or features would you want to develop, and how would you evaluate progress of the improved algorithm?
Social network data can be used to find more meaningful matches. With the social network data we can perform some natural language processing to understand the players likes & preferences.
In addition, we can use the pictures from the application to understand what kind of images get the most likes.
Models can be evaluated using cross-validation.

