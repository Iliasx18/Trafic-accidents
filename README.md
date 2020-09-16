# Trafic-accidents
Quick model that predicts the gravity of car accidents based on different features : circumstances, characteristics of road and passengers... 

Open data from 2018 provided by the French ministry of transport : [Link here](https://www.data.gouv.fr/fr/datasets/base-de-donnees-accidents-corporels-de-la-circulation/#)

We treat this as a 0-1 classification problem (1 being serious accident), the classes are imbalanced (only 16% of accidents are labeled as serious).
Used python and scikit-learn library for the implementation of logistic regression and gradient boosting classifier, then evaluated the model using classic metrics (accuracy, precision, recall...) and AUC for ROC and precision-recall curves.

For example, the results for the area under the precision-recall curve are :

|                         | AUC (Train)    | AUC (Test)  |
| ----------------------- |:--------------:|:-----------:| 
| Mean                    | 0.84           | 0.45        |
| Standard deviation      | 0.11           |       0.05  | 

Whereas the AUC score of a random classifier is around 16%
