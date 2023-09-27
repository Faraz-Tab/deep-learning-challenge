# Module 21 Report Template on the labled data set to compile and optimize a model in predicting weather or not an organization is successful after recieving funds from the charity.



Overview:
Weather or not an organization is successful depends on many factors but given our data set of the assignment, Firstly I prepared the data of the as instructed in our assignment and then split the data with a 3:1 ratio for the testing and training data sets. The purpose of the analysis is the get an accuracy score of at least 75% on the our testing predictions. I have used many mathods including PCA to find our what percentage of the data available can be eliminated without the risk of losing data.   


Results:

* What variable(s) are the target(s) for your model? 
  Our target is the binary data recorded in the "IS_SUCCESSFUL" column of the data set. 

* What variable(s) are the features for your model?
  On our normal model. I have selected every column except "Name" and "EIN" numbers as my features. But in my optimized model, I have further reduced "Status" and "Special_considerations" as they were not contributing value to our learning algorithms.

* What variable(s) should be removed from the input data because they are neither targets nor features?
  "Name" and "EIN" are columns that are neither targets nor Feature as they are unique data for each individual data point and do not contribute to our predictions.





* How many neurons, layers, and activation functions did you select for your neural network model?
  For our first model, I chose to go with two hidden layers, each containing 15 neurons. For our feature layer, I had 43 input dimentions and a single neuron with a "Sigmoid" activatio function as the target neuron since our target prediction id a binoary problem to solve.

  * Were you able to achieve the target model performance?
    I was not able to acheive the target accuracy performance even after optimization methods I used.

  * What steps did you take in your attempts to increase model performance?
  I tried PCA to reduce the dimentions, Decision forest to check for feature importance, I used tuning codes in a seperate colab jupyter notebook and even reduced "STATUS" and "SPECIAL_CONSIDERATION" columns. I used different test and training ratio splits and even tried to add duplicated data to our data set to further help the models accuracy. but none were helpful as the maximus accuracy I received was 74 percente on my training data and 72.3% on my testing data. I have even changed the activation functions between "Relu", "tanh" and even "Sigmoid". I added up to 5 hidden layer and a maximum of  2500 neurons spread in between the hidden layers but only further confused the accuracy. On my best performance, I got 74.3 % accuracy on my training data and a 73.8 % on my testing data. I could not achieve the target of 75%.


  summary:
  We could try to gather more columns and features to further help our model as the data itself is the most important part and what the machine recieves as input is the most important feature. I would recommend to further collect more imformation if available, or if not, trying other algorythms such as SVM or random forst might be better options to try. 