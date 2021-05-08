## Evaluation Metrics

```
Accuracy = total no. of correct predictions / total no. of observation
```
```
Precision = total no. of correct predictions / total no. of prediction
```
For False positive optimize model on Precision
```
Recall = total no. of correct predictions / total of observation that were supposed to be predicted
```
For False Negatives optimize model on Recall

## Optimal Model

||Underfitting|Good Model|Overfitting|
|---|---|---|---|
|**Complexity**|Low|Medium|High|
|**Bias**|High|Low|Low|
|**Variance**|Low|Low|High|
|**Train Error**|High|Low|Low|
|**Test Error**|High|Low|High|

## Model


#### Logistic Regression

##### Mainly Used for Regression and Prediction Problem

##### When to Use it?
* Binary target variable
* Transparency is important or interested in significance of predictors
* Fairly well-behaved data
* Need a quick initial benchmark

##### When Not to Use it?
* Continuous target variable
* Massive data (row or columns)
* Unwieldy data
* Performance is the only thing that matters



#### Support Vector Machine 

##### Mainly Used for Classification Problem

##### When to Use it?
* Binary target variable
* Feature-to-row ratio is high
* Very Complex relationships
* Lots of Outliers

##### When Not to Use it?
* Feature-to-row ratio low
* Transparency is important or interested in significance of predictors
* Looking for a quick benchmark model

#### Multi-Layer Perceptron

##### Could be Used for both Prediction and Classification

##### When to Use it?
* Categorical or continuous target variable
* Very complex relationships or performance is the only thing that matters
* When control over the training process is very important

##### When Not to Use it?
* Image recognition, time, series, etc.
* Transparency is important or interested in significance of predictors
* Need a quick benchmark model
* Limited data available

#### Random Forest

##### When to Use it?
* Categorical or continuous target variable
* Interested in significance of predictors
* Need a quick benchmark model
* If you have messy data, such as missing values, outliers

##### When Not to Use it?
* If you're solving a very complex, novel problem
* Transparency is important
* Prediction time is important

#### Gradient Boosting

##### When to Use it?
* Categorical or continuous target variable
* Useful on nearly any type of problem
* Interested in significance of predictors
* Prediction time is important

##### When Not to Use it?
* Transparency is important
* Training time is important or compute power is limited
* Data is really noisy



### Summary

|Accuracy|Latency|
|--|--|
|How do they handle data of different sizes, such as short and fat long and skinny?|How long will it take to train?|
|How will they handle the complexity of feature relationships?|How long will it take to predict?|
|How will they handle messy data?||

#### Model Classification

||Problem<br>Type|Train<br>Speed|Predict<br>Speed|Interpretability|Performance|Performance<br>with<br>Limited Data|
|---|---|---|---|---|---|---|
|**Logistic<br>Regression**|Classification|Fast|Fast|Medium|Lower|Higher|
|**Support Vector<br>Machines**|Classification|Slow|Moderate|Low|Medium|Higher|
|**Multi-Layer<br>Perceptron**|Both|Slow|Moderate|Low|High|Lower|
|**Regression Forest**|Both|Moderate|Moderate|Low|Medium|Lower|
|**Boosted Trees**|Both|Slow|Fast|Low|High|Lower|
