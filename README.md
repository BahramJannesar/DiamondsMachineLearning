## Diamonds

[Diamond](https://en.wikipedia.org/wiki/Diamond) is a solid form of the element carbon with its atoms arranged in a crystal structure called diamond cubic. At room temperature and pressure, another solid form of carbon known as graphite is the chemically stable form, but diamond almost never converts to it. Diamond has the highest hardness and thermal conductivity of any natural material, properties that are utilized in major industrial applications such as cutting and polishing tools. They are also the reason that diamond anvil cells can subject materials to pressures found deep in the Earth.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Image/GuideToDiamonds_LP_Hero_Desktop_v2-2.jpeg)

## Diamonds Dataset :

This classic dataset contains the prices and other attributes of almost 54,000 diamonds. It's a great dataset for machine learnung and work with data analysis and visualization.

### Dataset Columns :

 * **price** : price in US dollars ( $326 - $18,823 ) 

 * **carat** : weight of the diamond ( 0.2 - 5.01 )

 * **cut** : quality of the cut ( Fair , Good , Very Good , Premium , Ideal )

 * **color** : diamond colour, from J ( worst ) to D ( best )

 * **clarity** : a measurement of how clear the diamond is ( I1 (worst) ,SI2 ,SI1 ,VS2 ,VS1 ,VVS2 ,VVS1 ,IF (best))

 * **x** : length in mm ( 0 - 10.74 )

 * **y** : width in mm ( 0 - 58.9 )

 * **z** : depth in mm ( 0 - 31.8 )

 * **depth** : total depth percentage = z / mean( x, y ) = 2 * z / ( x + y ) --> ( 43 - 79 )

 * **table** : width of top of diamond relative to widest point ( 43 - 95 )
 
 ![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Image/Anglo-DiamondAnatomy_03.jpg)
 
 ## Machine Learning
 
On this dataset we used 2 methods of classic machine learining :

**1. Regression** 

**2. Classification** 

Used regression on all of the columns that were related to the **price** columns and for classification use all columns that were related to the **cut** column.

### Regression on this dataset :

Algorithms :
  
  * Lasso Regression
  * Linear Regression	
  * Ridge Regression
  * Adaboost Regressor
  * XGBRFRegressor
  * Decision Tree Regressor
  * Gradient Boosting Regressor
  * Bagging Regressor
  * Random Forest Regressor
  * XGB Regressor
  * Extra Trees Regressor
 
 ![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/Accuracy%20Reg.png)
 
  The best accuracy between these algorithms is **98.16 %** with **ExtraTreesRegressor**.
 
#### Lasso Regression :

Lasso (least absolute shrinkage and selection operator; also Lasso or LASSO) is a regression analysis method that performs both variable selection and regularization in order to enhance the prediction accuracy and interpretability of the statistical model it produces. It was originally introduced in geophysics literature in 1986.

Lassso Regression with **90.5659 %** accuray is the worst algorithm for this dataset.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/Lasso%20Reg.png)

As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did not cover each other well. 
 
#### Linear Regression :

Linear regression is a linear approach to modeling the relationship between a scalar response (or dependent variable) and one or more explanatory variables (or independent variables). The case of one explanatory variable is called simple linear regression. 

Linear Regression with **90.5664 %** accuray and with **0.0005 %** difrence with Lasso Regression is one the worst algorithm for this dataset.

 ![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/LinearReg.png)
 
As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did not cover each other well like Lasso Regression.
 
#### Ridge Regression :

Tikhonov regularization, named for Andrey Tikhonov, is a method of regularization of ill-posed problems. Also known as ***ridge regression***,it is particularly useful to mitigate the problem of multicollinearity in linear regression, which commonly occurs in models with large numbers of parameters.In general, the method provides improved efficiency in parameter estimation problems in exchange for a tolerable amount of bias (see bias–variance tradeoff).
 
Ridge Regression with **90.5666 %** accuray and with **0.0002 %** difrence with Linear Regression is one the worst algorithm for this dataset.
 
![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/RidgeReg.png)

As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did not cover each other well like Linear Regression.

#### Adaboost Regressor :

AdaBoost, short for Adaptive Boosting, is a machine learning meta-algorithm formulated by Yoav Freund and Robert Schapire, who won the 2003 Gödel Prize for their work. It can be used in conjunction with many other types of learning algorithms to improve performance. The output of the other learning algorithms ('weak learners') is combined into a weighted sum that represents the final output of the boosted classifier.

Adaboost Regressor with **91.87 %** accuray is on the fouth place of this list.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/Adaboost%20Reg.png)

As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did not cover each others good.

#### XGBRF Regressor and XGB Regressor :

XGBoost is an optimized distributed gradient boosting library designed to be highly efficient, flexible and portable.
It implements machine learning algorithms under the Gradient Boosting framework. XGBoost provides a parallel tree
boosting (also known as GBDT, GBM) that solve many data science problems in a fast and accurate way.
 
XGBRF Regressor with **96.28 %** accuray is on the fifth place of this list.
XGB Regressor with **98.15 %** accuray is one the best algorithm for this datast and is on the ninth place of this list.
 
 #### Decision Tree Regressor :
 
Decision tree learning is one of the predictive modelling approaches used in statistics, data mining and machine learning. It uses a decision tree (as a predictive model) to go from observations about an item (represented in the branches) to conclusions about the item's target value (represented in the leaves). Tree models where the target variable can take a discrete set of values are called classification trees; in these tree structures, leaves represent class labels and branches represent conjunctions of features that lead to those class labels. Decision trees where the target variable can take continuous values (typically real numbers) are called regression trees.

Decision Tree Regressor with **96.72 %** accuray is on the sixth place of this list.
 
![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/Decision%20Tree%20Reg.png)

As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did not cover each others good.

#### Gradient Boosting Regressor :

Gradient boosting is a machine learning technique for regression and classification problems, which produces a prediction model in the form of an ensemble of weak prediction models, typically decision trees. It builds the model in a stage-wise fashion like other boosting methods do, and it generalizes them by allowing optimization of an arbitrary differentiable loss function.

Gradient Boosting Regressor with **97.66 %** accuray is on the sixth place of this list.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/GBR.png)

As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did not cover each better than the others algorithms.

#### Bagging Regressor :

Bootstrap aggregating, also called bagging (from bootstrap aggregating), is a machine learning ensemble meta-algorithm designed to improve the stability and accuracy of machine learning algorithms used in statistical classification and regression. It also reduces variance and helps to avoid overfitting. Although it is usually applied to decision tree methods, it can be used with any type of method. Bagging is a special case of the model averaging approach.

Bagging Regressor with **97.96 %** accuray and with **0.30 %** difrence with Gradient Boosting Regressor is one the best algorithm for this dataset.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/Bagging%20Reg.png)


As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did cover each better than the others algorithms.

#### Random Forest Regressor :

Random forests or random decision forests are an ensemble learning method for classification, regression and other tasks that operate by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees .Random decision forests correct for decision trees' habit of overfitting to their training set.

Random Forest Regressor with **98.14 %** accuray is one the best algorithm that we ran.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/Random%20Forest%20Reg.png)

As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did cover each better than the others algorithms.

#### Extra Trees Regressor :

The Extra-Tree method (standing for extremely randomized trees) was proposed in [GEW06](https://orbi.uliege.be/handle/2268/9357), with the main objective of further randomizing tree building in the context of numerical input features, where the choice of the optimal cut-point is responsible for a large proportion of the variance of the induced tree.

Random Forest Regressor with **98.16 %** accuray is the best algorithm that we ran.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Regression/Extra%20Trees%20Reg.png)

As you can see on this diagram that show only 200 first record of dataset , the values of the **y_pred** and **y_test** did cover each other well.

### Classification on this dataset :

Algorithms :
  
  * kNN ( k-Nearest Neighbors )
  * SVM ( Sub Vector Machine )
  * Logistic Regression

The best accuracy between these algorithms is **75.27 %** with **SVM** but this algorithm with cv parameter equal 5 has very long time for learing like 4 hours.

#### kNN ( k-Nearest Neighbors ) :

In pattern recognition, the k-nearest neighbors algorithm (k-NN) is a non-parametric method used for classification and regression.[1] In both cases, the input consists of the k closest training examples in the feature space.

One the important part of the kNN algorithm is to find the best k for learning we try these parameter and choose the best one of them.

**1. First test :**

 * test_size = 30 %
 
 * random_state = 42
 
![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/1.png)

**2. Second test :**

 * test_size = 20 %
 
 * random_state = 21
 
![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/2.png)

**3. Third test :**

 * test_size = 30 %
 
 * random_state = 21
 
![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/3.png)

**4. Fourth test :**

 * test_size = 40 %
 
 * random_state = 21
 
![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/4.png)

**5. Fifth test :**

 * test_size = 40 %
 
 * random_state = 42
 
![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/5.png)

**6. Six test :**

 * test_size = 20 %
 
 * random_state = 42
 
![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/6.png)


kNN ( k-Nearest Neighbors ) with k = 8 and **65.85 %** accuray is better than Logistic Regression.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/knn.png)

The **confusion matrix** of kNN :

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/knn_cf.png)

Apart from the main diameter of the matrix. we see that the rest of the matrix is also inclined to dark color and shows the low accuracy of this algorithm.

#### SVM ( Sub Vector Machine ) :

In machine learning, support-vector machines (SVMs, also support-vector networks[1]) are supervised learning models with associated learning algorithms that analyze data used for classification and regression analysis. Given a set of training examples, each marked as belonging to one or the other of two categories, an SVM training algorithm builds a model that assigns new examples to one category or the other, making it a non-probabilistic binary linear classifier (although methods such as Platt scaling exist to use SVM in a probabilistic classification setting). An SVM model is a representation of the examples as points in space, mapped so that the examples of the separate categories are divided by a clear gap that is as wide as possible. New examples are then mapped into that same space and predicted to belong to a category based on the side of the gap on which they fall.

SVM ( Sub Vector Machine ) with **75.27 %** accuray is the best algorithm that we ran.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/svm.png)

The **confusion matrix** of SVM :

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/svm_cf.png)

Apart from the main diameter of the matrix. we see that the rest of the matrix is better than the others alogirthms confusion matrix. 


#### Logistic Regression :

the logistic model (or logit model) is used to model the probability of a certain class or event existing such as pass/fail, win/lose, alive/dead or healthy/sick. This can be extended to model several classes of events such as determining whether an image contains a cat, dog, lion, etc. Each object being detected in the image would be assigned a probability between 0 and 1 and the sum adding to one.

Logistic Regression with **65.00 %** accuray is the worst algorithm that we ran.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/LogisticReg.png)

The **confusion matrix** of SVM :

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Accuracy%20Classification/LogisticReg_cf.png)

Apart from the main diameter of the matrix. we see that the rest of the matrix is also inclined to dark color and shows the low accuracy of this algorithm.

### Writers 

* [Soursh Ghaderi](https://github.com/SoroushGhaderi) ( :pencil2: )

* [Bahram Jannesar](https://github.com/BahramJannesar) ( :pencil2: )

