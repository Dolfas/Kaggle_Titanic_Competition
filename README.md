## What is this project all about?
In this all-time starter for Kaggle competitions, I used machine learning for the prediction of the survival of Titanic passengers based on features like sex and age.
With this in mind, I used Random Forests since they are suitable for tabular data.

<p align = "center">
  <img src="https://cdn.britannica.com/79/4679-050-BC127236/Titanic.jpg" width="450" >
</p>

You can obtain the data used <a href="https://www.kaggle.com/competitions/titanic/data">here</a>.

## Random Forests
Random forests consist of an ensemble of multiple decision trees, that are made to be as uncorrelated as possible with each other. In order to obtain such uncorrelation, two methods are employed: <strong>Bootstrap Aggregation</strong> and <strong>Feature Bagging</strong>. Bootstrap Aggregation allows you to randomly sample, with replacement, data from the training dataset to make each decision tree. Additionally, Feature Bagging specifies what features each decision tree can use for splitting nodes. 

Accordingly, the best hyperparameters for the Random Forest were found using <i>gridsearch</i>:

 <ul>
  <li><strong>Criterion</strong> = 'gini' (The Criterion evaluates each possible feature-based split)</li>
  <li><strong>max_depth</strong> = 8 (The max_depth sets the maximum size of each decision tree)</li>
  <li><strong>max_features</strong> = 'sqrt' (The max_features conditions what features can be used by each decision tree)</li>
  <li><strong>max_leaf_nodes</strong> = 6 (The max_leaf_nodes sets the maximum number of leaf nodes that each decision tree can have)</li>
  <li><strong>n_estimators</strong> = 100 (The n_estimators defines the number of decision trees present in our Random Forest)</li>
</ul> 

## Results
Finally, the results for this Random Forest were:

<p align = "center">
  <img src="https://github.com/Dolfas/Kaggle_Titanic_Competition/assets/80644787/7a474fed-a5c2-4cb7-9bf1-73ea1be14c58" width="750" >
</p>



