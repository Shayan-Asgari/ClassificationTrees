![tree](https://user-images.githubusercontent.com/31261309/50881439-69a5b380-1396-11e9-9e37-0e2873bd529c.png)


# ClassificationTrees
Comparing and exploring results of a Decision Tree vs. a Random Decision Tree to predict outcome of a label. I explored an open data source from the Lending Club prior to their scandal to see if I could determine if the features such as FICO, interest rates, etc. would impact whether or not a customer of the Lending Club was able to pay back their loans. In this project, the result was categorical in nature and essentially in a Machine Learning Model had to be numerical, thus following 1's and 0's depicting YES or NO. 

## Background Information

Algorithm: 

The Decision Tree algorithms is a frequency based algorithm that can be used for regression or classification. Decision Trees uses different criteria to create nodes (split based on a certain attribute) which then creates edges (condition <74 or >74) and leaves (the result).
The Random Forests algorithm uses a bagging concept which is nothing more than bootstrap aggregation. The idea of bagging is to build many models with low bias and high variance, then average them which balances the bias-variance trade off. 

Similarities: 

Random Forests extremely similar to Decision Trees in that they are a collection/ensemble of Decision Trees. 

Differences: 

While Decision Trees use all the features and variables that interest us to determine a result, Random Trees randomly selects features to make multiple Decision Trees and average the results as the output of the Random Trees. Random trees are also trained independently from another. Essentially N trees are selected randomly with replacement where samples are drawn from the main data set and these n data sets work in parallel to give you a solution based on the simple majority of the average. 

Benefits of Decision Tree:

Benefits of using a Decision Tree is that it does not require much data preprocessing nor does it require knowing the distribution of the data. They are also fast, perform well on big data sets and easy to interpret.

Disadvantages: 

Prone to overfitting when tree is too deep (fits training data very well but not test set). Overfitting is the tendency for the model of the data to be too exactly related to a particular set of data which causes the model to be unable to predict future observations reliably. Overfitting occurs when there is low bias and high variance. 
   
Benefit of Random Forest: 

A benefit to using Random Forests is that it helps reduce variance by reducing the overfitting of data SINCE it averages out the result of other trees. They also limit error due to bias and variance as the sample size increases. By training random sample data, the model ensures that the base trees of the model will not become too highly correlated. By using the process of bagging, there will be an abundance of randomly generated training data so that it produces multisets of the same size of the original data. By increasing the size of the training data, we decrease the variance by tuning our predictions. If the test set is ran on a model built by various/random training data to produce predictions which are then averaged, it will be more accurate and vary less than the overfitting that would be possibly created by a Decision Tree.

Disadvantages:

- Model is too complex to interpret
- By limiting part of data to use and limiting number of variables to split on the for each of the individual trees, bias increases, however, because the results are averaged, we see the bias decrease.

Links for more Information: 
1. https://towardsdatascience.com/decision-trees-and-random-forests-df0c3123f991
2. https://www.linkedin.com/pulse/decision-tree-vs-random-forest-ankita-paunikar/

## Prerequisites 
* Jupyter Notebook
* Python Programming Experience

## Installation 
1. Seaborn
2. NumPy
3. Pandas
4. Matplotlib
5. Sklearn

## Contribute
1. Fork it 
2. Commit your changes 
3. Push to the branch 
4. Create Pull Requests

## Acknowledgements
* Curiousity and admiration for Machine Learning
* Udemy
