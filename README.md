# PUBG-win_place-prediction

AIM

The goal of this project is to develop a machine learning algorithm on the real world PUBG dataset to predict the the finishing rank of all one hundred players participating in the match based on their end game statistics. Also, another aim of this project is to do exploratory data analysis on PUBG game data to check out interesting findings such as which strategies which is most successful at winning. 

DATA

We have PUBG or Player Unknown Battleground’s anonymized player data of over 65,000 games with more than 30 attributes or features. Kaggle has given us PUBG mobile game statistics where each row represents one player’s after game statistics. Since PUBG’s data is already cleaned and pre-processed so there is no need for it. 

Reference : "https://www.kaggle.com/c/pubg-finish-placement-prediction/data"

ANALYSIS

In exploratory data analysis of the PUBG real world dataset, first analyse different player strategies such as killing and running. Also analyse how these strategies or attributed are correlated to the the variable we have to predict i.e player rank (winPlacePerc).

PREDICTION

Method:
First calculate the correlation to find out the whether there is relationship between attributes and the target “winPlacePerc”.
Secondly, we would do feature engineering on the data to create 10 new attributes that would help improve our model.
Next would be training our machine learning model on our feature set to predict the the finishing rank of players in our dataset.

TRAINING

I took a sample of 500,000 rows from our dataset for training our algorithm and the machine learning algorithm that I use for this problem is Random Forest. Random Forest is an ensemble of many decision tree algorithms that works with both classification and regression problems. Even without tuning the hyperparameters it gives great results all the time.

Feature Importance:
A feature of random forest algorithm is feature importance. Feature importance ranks the relative importance of every attribute for the prediction. The feature importance function I use from sklearn library calculates importance of attributes by seeing how much the tree nodes, that use that attribute, amount for reduction in entropy across all trees in the random forest.
