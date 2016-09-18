## The Curse of Dimensionality

As the number of features or dimensions grows, the amount of data we need to generalize accurately grows **exponetially**.

## Learning curves

A learning curve is a graph that compares the performance of a model on training and testing data over a varying number of training instances.

When we look at the relationship between the amount of training data and performance, we should generally see performance improve as the number of training points increases.

By separating training and testing sets and graphing performance on each separately, we can get a better idea of how well the model can generalize to unseen data.

A learning curve allows us to verify when a model has learned as much as it can about the data. When this occurs, the performance on both training and testing sets plateau ad there is a consistent gap between the two error rates.

### Bias

When the training and testing errors converge and are quite high this usually means the model is biased. No matter how much data we feed it, the model cannot represent the underlying relationship and therefore has systematic high errors.

### Variance

When there is a large gap between the training and testing error this generally means the model suffers from high variance. Unlike a biased model, models that suffer from variance generally require more data to improve. We can also limit variance by simplifying the model to represent only the most important features of the data.

## Ideal Learning Curve
The ultimate goal for a model is one that has good performance that generalizes well to unseen data. In this case, both the testing and training curves converge at similar values. The smaller the gap between the training and testing sets, the better our model generalizes. The better the performance on the testing set, the better our model performs.

## Model Complexity
The visual technique of graphing performance is not limited to learning. With most models, we can change the complexity by changing the inputs or parameters.

A model complexity graph looks at training and testing curves as the model's complexity varies. The most common trend is that as a model increases, bias will fall off and variance will rise.
