# Hyperparameter-tuning-Random-Forest
Car Evaluation Database is used to predict Class based on features. Hyperparameter tuning is done using Grid Search and Random search.

Random forest has multiple parameters and selecting the right set of parameteres can be tricky. Hyperparameter tuning is adjusting right set of parameters to achieve maximum accuracy and high precision. In the code I adjust following parameters in random forest:

1. max_depth: maximum depth or extent to which I want an individual tree in my random forest to grow.
2. min_sample_split: a hyperparameter that tells the decision tree in a random forest the minimum required number of observations in any given node after split from parent node. 
3. max_leaf_nodes: a hyperparameter sets a condition on the splitting of the nodes in the tree and hence restricts the growth of the tree. 
4. min_sample_leaf: this hyperparameter specifies the minimum number of samples that should be present in the leaf node after splitting a node.
5. n_estimtors: number of trees to be created in Random forest model.
6. max_samples: it determines what fraction of the original dataset is given to any individual tree while bootstrapping from the parent dataset.
7. bootstrap: True or False. The default value of bootstrap is True but to disable the bootstrap we can assign it as False and the whole dataset will be considered for the formation of Decision Trees.
6. max_features: This denotes the maximum number of features to be considered while bootstrapping.

For this model I use 2 methods of hyperparameter tuning:

1. Random Search using Cross Validation - Random search is a technique where random combinations of the hyperparameters are used to find the best solution for the built model.

2. Grid Search - We use existing list of parameters to tune the model and as the model accuracy converges to maximum, those set of parameters are chosen.
