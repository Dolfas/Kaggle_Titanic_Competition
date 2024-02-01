## What is this project all about?
In this all time starter for kaggle competitions, I used machine learning for the prediction of the survival of titanic passengers based on features like sex and age. 
With this intent I used Random Forests, since they are suitable for tabular data.

<p align = "center">
  <img src="https://cdn.britannica.com/79/4679-050-BC127236/Titanic.jpg" width="450" >
</p>

You can obtain the data used here (link to kaggle).

## Random Forests
Random forests consist on an ensemble of multiple decision trees, which are made to be as uncorrelated as posible with each other. In order to obtain such uncorrelation two methods are employed: <strong> Bootstrap Aggregation </strong> and <strong> Feature Bagging</strong>.Bootstrap Aggreagation allows to randomly sample, with replacement, data from the training data set to make each decision tree. Additionally, Feature Bagging conditions the number of features that each decision tree can use for splitting. 

Accordingly, the best hyperparameters of the used Random Forest were found using <i>gridsearch</i>:

 <ul>
  <li><strong>Criterion</strong> = 'gini' (The Criterion evaluates each possible feature based split)</li>
  <li><strong>max_depth</strong> = 8 (The max_depth sets the maximum size of each decision tree)</li>
  <li><strong>max_features</strong> = 'sqrt' (The max_features conditions what features can be used by each decision tree)</li>
  <li><strong>max_leaf_nodes</strong> = 6 (The max_leaf_nodes sets the maximum number of leaf nodes each decision tree can have)</li>
  <li><strong>n_estimators</strong> = 100 (The n_estimators defines the number of decision trees present in our Random Forest)</li>
</ul> 

## Results
Finally, we obtained the following results after submiting our csv in kaggle:
