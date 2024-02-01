## What is this project all about?
In this all time starter for kaggle competitions, I used machine learning for the prediction of the survival of titanic passengers based on features like sex and age. 
With this intent I used Random Forests, since they are suitable for tabular data.

<p align = "center">
  <img src="https://cdn.britannica.com/79/4679-050-BC127236/Titanic.jpg" width="450" >
</p>


## Random Forests
Random forests consist on an ensemble of multiple decision trees, which are made to be as uncorrelated as posible with each other. In order to obtain such uncorrelation two methods are employed: <strong> Bootstrap Aggregation </strong> and <strong> Feature Bagging</strong>.Bootstrap Aggreagation allows to randomly sample, with replacement, data from the training data set to make each decision tree. Additionally, Feature Bagging conditions the number of features that each decision tree can use for splitting. 

Accordingly, the best hyperparameters of the used Random Forest were found using <i>gridsearch</i>:

 <ul>
  <li><strong>Criterion</strong> = 'gini' </li>
  <li><strong>max_depth</strong> = 8 </li>
  <li><strong>max_features</strong> = 'sqrt' </li>
  <li><strong>max_leaf_nodes</strong> = 6 </li>
  <li><strong>n_estimators</strong> = 100 </li>
</ul> 

## Results

