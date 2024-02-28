# Pokemon Data Classification Accuracy
In this project, we will classify based on the accuracy level using pokemon data.

## Dataset
This dataset contains information on all 800 Pokemon from all Seven Generations of Pokemon. The information contained in this dataset includes:
- Num: ID for each Pokémon.
- Name: Name of each Pokémon.
- Type1: Each Pokémon has a type, this determines weakness/resistance to attacks.
- Type2: Some Pokémon are dual type and have 2.
- Total: Total of Pokémon.
- HP: Hit points, or health, defines how much damage a Pokémon can withstand before fainting.
- Attack: The base modifier for normal attacks (eg. Scratch, Punch).
- Defense: The base damage resistance against normal attacks.
- SPAtk: Special attack, the base modifier for special attacks (e.g. fire blast, bubble beam).

## Classification
Classification belongs to supervised learning algorithms, algorithms that rely on labeled input data to learn a function that provides the appropriate output when given new unlabeled input data.

The prediction accuracy of a classification algorithm can be seen in the confusion matrix. Confusion matrix is used for classification problems where the output can be two or more classes. Confusion matrix is a table containing four different permutations of predicted and actual values.
![NaiveBayesClassification](https://github.com/salmafirdausi/pokemondataset/blob/d0a7e3fc86160fd02aebeb68af7783758fa2aa5d/confusionMatrix.png)

Notes:
- TP is the number of positive cases classified as positive,
- FP is the number of negative cases classified as positive,
- TN is the number of negative cases classified as negative,
- FN is the number of positive cases classified as negative.

Classification performance can be evaluated by looking at the following measures.
### 1. Classification accuracy
Accuracy is the share of correctly classified objects in the total number of objects. In other words, it indicates how often the model is correct overall.
Where TP = True Positives, TN = True Negatives, FP = False Positives, and FN = False Negatives.

Accuracy alone doesn't tell the full story when you're working with a **class-imbalanced data set**, where there is a significant disparity between the number of positive and negative labels. Metrics for evaluating class-imbalanced problems are precision and recall.

### 2. Confusion matrix

A confusion matrix is a tool for summarizing the performance of a classification algorithm. A confusion matrix will give us a clear picture of classification model performance and the types of errors produced by the model. It gives us a summary of correct and incorrect predictions broken down by each category. The summary is represented in a tabular form.

Four types of outcomes are possible while evaluating a classification model performance. These four outcomes are described below:-

+ **True Positives (TP)** – True Positives occur when we predict an observation belongs to a certain class and the observation actually belongs to that class.
+ **True Negatives (TN)** – True Negatives occur when we predict an observation does not belong to a certain class and the observation actually does not belong to that class.
+ **False Positives (FP)** – False Positives occur when we predict an observation belongs to a certain class but the observation actually does not belong to that class. This type of error is called Type I error.
+ **False Negatives (FN)** – False Negatives occur when we predict an observation does not belong to a certain class but the observation actually belongs to that class. This is a very serious error and it is called Type II error.

### 3. Classification Report
Classification report is another way to evaluate the classification model performance. It displays the precision, recall, f1 and support scores for the model. 

### 4. Precision
Precision can be defined as the percentage of correctly predicted positive outcomes out of all the predicted positive outcomes. It can be given as the ratio of true positives (TP) to the sum of true and false positives (TP + FP).

So, Precision identifies the proportion of correctly predicted positive outcome. It is more concerned with the positive class than the negative class.

Mathematically, precision can be defined as the ratio of TP to (TP + FP).

### 5. Recall
Recall can be defined as the percentage of correctly predicted positive outcomes out of all the actual positive outcomes. It can be given as the ratio of true positives (TP) to the sum of true positives and false negatives (TP + FN). Recall is also called Sensitivity.

Recall identifies the proportion of correctly predicted actual positives.

Mathematically, recall can be given as the ratio of TP to (TP + FN). True Positive Rate is synonymous with Recall and can be given as the ratio of TP to (TP + FN).

### 6. F1-score
F1-score is the weighted harmonic mean of precision and recall. The best possible F1-score would be 1.0 and the worst would be 0.0. F1-score is the harmonic mean of precision and recall. So, F1-score is always lower than accuracy measures as they embed precision and recall into their computation. The weighted average of F1-score should be used to compare classifier models, not global accuracy.



## Model Building
### 1. Regression Logistic
Logistic Regression is a regression analysis used to describe the relationship between a response variable and a set of predictor variables where the response variable is binary or dichotomous.

### 2. Decision Tree
Decision Tree is a structure similar to a flow chart. In a Decision Tree, each internal node (a node that is not a leaf node or not the outermost node) is a test for an attribute variable, each branch is the result of the test, and the leaf, which is the outermost node, becomes a label.

### 3. Random Forest
The random forest method is an extension of the CART method, by applying bootstrap aggregating and random feature selection methods. In random forest, many trees are grown so that a forest is formed, then analysis is carried out on the collection of trees.

### 4. Naïve Bayes
Naïve Bayes is a direct probabilistic classification technique that calculates a set of probabilities by combining frequencies and combinations of values from a given data set. The algorithm uses Bayes' theorem and assumes all attributes are independent or not interdependent given the value of the class variable.

### 5. KNN
The KNN method is one of the easiest classification techniques. It identifies k patterns that are most similar to the input pattern, and then determines the decision class based on the number of patterns. The KNN train process produces k with optimal generalization accuracy for future data.

### 6. SVM
SVM is used for linearly separable data, which means if a dataset can be classified into two classes using a single straight line. The SVM method aims to find the optimal hyperplane. The hyperplane that can divide the two classes with the furthest margin distance between classes. Margin is the distance between the hyperplane and the closest pattern from each class. The closest instance is called the support vector.
