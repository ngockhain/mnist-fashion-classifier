# Mnist-fashion-classifier
Classifier object with mnist dataset
## Quá trình cải tiến mô hình để có được kết quả tốt nhất.
How does student do this lab?
-> Student uses 4 algorithms to train on train set and evaluate on test set. Student change the parameters on each algorithm to get the best accuracy.
- 4 algorithms used is: SGDClassifier, ExtraTreeClassifier, DecisionTreeClassifier, MLPClassifier.
### 1. SGDClassifier:
- Student used set of params: {penalty: [l1, l2]} and cross validation = 5 on the training set.
- And then get the best params:
- With accuracy: 
### 2. ExtraTreeClassifier:
- Student used set of params: {splitter: ['best', 'random'], max_depth:[10,50,100], criterion:['gini', 'entropy']} and cross validation = 5 on the training set.
- And then get the best params:
- With accuracy: 
### 3. DecisionTreeClassifier:
- Student used set of params like in <b>ExtraTreeClassifier</b>: {splitter: ['best', 'random'], max_depth:[10,50,100], criterion:['gini', 'entropy']} and cross validation = 5 on the training set.
- And then get the best params:
- With accuracy: 
### 4. MLPClassifier:
- Student used set of params: {hidden_layer_sizes: [10,50,100], activation: ['tanh', 'relu']} and cross validation = 5 on the training set.
- And then get the best params:
- With accuracy: 
