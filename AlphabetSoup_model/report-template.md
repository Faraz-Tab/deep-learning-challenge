# Module 21 Report Template

## Overview of the Analysis



* Explain the purpose of the analysis.


* Explain what financial information the data was on, and what you needed to predict.


* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).


* Describe the stages of the machine learning process you went through as part of this analysis.


* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  After oversampling the training data, Our second model still performs the same with the only difference being the recall score for our unhealthy data which goes up to 99%. This is though to the fact that our negative leans data points have been increased drastically which affects this number. how ever, the precision score is even lower and we can see that the number of our False negatives has even increased. This is though to the data points being copied and is not only overfitting the model, but resulting in a false 4$ increase inour accuracy. 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
Between the two models, I still think our first model is more accurate in being generalized and our second model is overfitted. even though it has a high accuracy.


* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
In this case, it is important to predint both of these loans, as our precision to correctly guress the  healthy loans, results in better predicrion of creditworthyness of future borrowers. And the precision in identifying unhealthy loans results in less loss and they both have a direct role to play in minimzing the default loss of the company. So in conclusion, our it is important to look at our f-1score score. 

If you do not recommend any of the models, please justify your reasoning.
In this report I can conclude that our models are not satisfactory in meeting with the correct requirments. both our mdoels do well with predicting healthy loans. But when it comes to accurately predicting our unhealthy data, their procision falls to an average of 85%. which then affects our f1-score. My recommendations for further investing into these machin learning models is to try using a differnet approach like using random forest or if possible, add extra columns(features) to our data set which might help to imporve our models accuracy in deperating these unhealthy data points and increast our precision for unhealthy loans. And lastly, the most reliable solution to increase our models accurace is to add more unhealhty samples to our data sets to further increase the precision and there for the overall accuracy of our model.

