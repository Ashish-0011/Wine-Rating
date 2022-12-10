# Wine-Rating
## To determine the quality of wine using different features like alcohol, citric acid etc.


The quality is defined from 3-8 where each rating is a class in itself. There are numerous features over which the quality is dependent i.e. alcohol, volatile acidity etc.
So the problem is a multiclass classification which can be approached through various ways, but here I have used particularly two algorithm i.e. Random forest and ADA Boost technique. 
We have used Correlation and through correlation we can determine the features which are highly correlated to the quality of wine. The features that are of importance are alcohol, volatile acidity, citric acidity and sulphates. We have removed the outliers from those specific features.

To determine accuracy with different combination features, we will be working in following way:
1) All of the Features
2) 4 Features i.e. alcohol, volatile acidity, citric acidity and sulphates
3) 2 Features i.e. alcohol, volatile acidity(Highest Correlation)

## Random Forest Classifier

1) All Features gives accuracy of 0.724
2) 4 features gives accuracy of 0.707
3) 2 features gives accuracy of 0.6

Through this, we decided to go use all the features as our training set.
Now using Grid Search CV, we tuned the hyperparameters, the accuracy turned out to be 71.724% which is less than before tuning but our model is robust in this case	
Then, the confusion matrix is used so that one can determine the number of misclassifications.

## ADA BOOST CLASSIFIER

1) All Features gives accuracy of 0.738
2) 4 features gives accuracy of 0.728
3) 2 features gives accuracy of 0.61
From above accuracies, we decided to go use all the features as our training set.
Now using Grid Search CV, we tuned the hyperparameters, the accuracy turned out to be 73.448% which is less than before tuning but our model is robust in this case.
Then the confusion matrix is used to determine the number of misclassifications.

# Conclusion
1) Using random forest classifier, we were able to obtain 71.24% accuracy of this model, which is a decent amount of accuracy.
2) Using ADA Boost classifier, we were able to obtain 73.448% accuracy of this model, which is decent as well.









