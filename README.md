## Diamonds

[Diamond](https://en.wikipedia.org/wiki/Diamond) is a solid form of the element carbon with its atoms arranged in a crystal structure called diamond cubic. At room temperature and pressure, another solid form of carbon known as graphite is the chemically stable form, but diamond almost never converts to it. Diamond has the highest hardness and thermal conductivity of any natural material, properties that are utilized in major industrial applications such as cutting and polishing tools. They are also the reason that diamond anvil cells can subject materials to pressures found deep in the Earth.

![](https://github.com/BahramJannesar/DiamondsMachineLearning/blob/master/Image/GuideToDiamonds_LP_Hero_Desktop_v2-2.jpeg)

## Diamonds Dataset 

This classic dataset contains the prices and other attributes of almost 54,000 diamonds. It's a great dataset for machine learnung and work with data analysis and visualization.

### Dataset Columns:

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

**1.Regression** 

**2.Classification** 

Used regression on all of the columns that were related to the **price** columns and for classification use all columns that were related to the **cut** column.

### Regression on this dataset:

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
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
