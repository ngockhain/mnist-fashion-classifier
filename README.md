# Mnist-fashion-classifier
Classifier object with mnist dataset
## Process of improvement model to get the best model.
How does student do this lab?<br/>
-> Student uses 4 algorithms to train on train set and evaluate on test set. Student change the parameters on each algorithm to get the best accuracy.
- 4 algorithms used is: SGDClassifier, ExtraTreeClassifier, DecisionTreeClassifier, MLPClassifier.
### 1. SGDClassifier:
- Student used set of params: `{penalty: [l1, l2]}` and cross validation = 5 on the training set.
- And then get the best params: `{penalty: l1}`
- With accuracy: 0.8136166666666667
### 2. ExtraTreeClassifier:
- Student used set of params: `{splitter: ['best', 'random'], max_depth:[10,50,100], criterion:['gini', 'entropy']}` and cross validation = 5 on the training set.
- And then get the best params: `{splitter: best, max_depth:10, criterion: entropy}`
- With accuracy: 0.7876833333333333
### 3. DecisionTreeClassifier:
- Student used set of params like in <b>ExtraTreeClassifier</b>: `{splitter: ['best', 'random'], max_depth:[10,50,100], criterion:['gini', 'entropy']}` and cross validation = 5 on the training set.
- And then get the best params: `{criterion: entropy, max_depth: 10, splitter: best}`
- With accuracy: 0.8126
### 4. MLPClassifier:
- Student used set of params: `{hidden_layer_sizes: [10,50,100], activation: ['tanh', 'relu']}` and cross validation = 5 on the training set.
- And then get the best params: `{activation: relu, hidden_layer_sizes:100}`
- With accuracy: 0.8558833333333333
#### After all, student choose MLPClassifier with best params to build programs to classified fashion object. Because it has biggest accuracy over 4 algorithms.
