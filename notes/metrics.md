Metrics
=======

# Metrics for Classification

## Accuracy
accuracy = (right guesses) / (total cases)

Accuracy is not the right metric in some cases, specially in skewed datasets,
or when errors are preferable on one side.

## Confusion matrix

```
       Actual  T   F
Predicted    
             -----------
 T           | TP | FP |
             ----------|
 F           | FN | TN |
             -----------
```

P = TP + FN
N = TN + FP

PP = TP + FP
NN = TN + FN

## Recall | Sensitivity

TP/P

- Fraction of positives which are found.
- Probability that a relevant item is retrieved.

## Precision

TP / (TP + FP)


- Proportion of relevant items which really are relevant.

## F1 score | balanced F score | F-measure

F1 score combines precision and recall relative to a specific positive class.

The F1 score can be interpreted as a weighted average of the precision and recall, where an F1 score reaches its best value at 1 and worst at 0:

F1 = 2 * (precision * recall) / (precision + recall)

For more information about F1 score how to use it in sklearn, check out the documentation here.

# Metrics for Regression

## Mean Absolute Error

One way to measure error is by using absolute error to find the predicted distance from the true value. The mean absolute error takes the total absolute error of each example and averages the error based on the number of data points. By adding up all the absolute values of errors of a model we can avoid canceling out errors from being too high or below the true values and get an overall error metric to evaluate the model on.

## Mean Square Error

Mean squared is the most common metric to measure model performance. In contrast with absolute error, the residual error (the difference between predicted and the true value) is squared.

Some benefits of squaring the residual error is that error terms are positive, it emphasizes larger errors over smaller errors, and is differentiable. Being differentiable allows us to use calculus to find minimum or maximum values, often resulting in being more computationally efficient.

## R^2 (coefficient of determination) regression score function.

Best possible score is 1.0 and it can be negative (because the model can be arbitrarily worse). A constant model that always predicts the expected value of y, disregarding the input features, would get a R^2 score of 0.0.

## Explained variance score

Best possible score is 1.0, lower values are worse.

