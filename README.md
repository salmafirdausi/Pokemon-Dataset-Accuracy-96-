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

## Lribaries


## Classification
Classification belongs to supervised learning algorithms, algorithms that rely on labeled input data to learn a function that provides the appropriate output when given new unlabeled input data.

The prediction accuracy of a classification algorithm can be seen in the confusion matrix. Confusion matrix is used for classification problems where the output can be two or more classes. Confusion matrix is a table containing four different permutations of predicted and actual values.

|  | Prediction |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |

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
