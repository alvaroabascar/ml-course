## Crossvalidation

We split our data into k subsets (k-fold cross-validation), and we run k separate experiments. For each subset, we take it as testing data and the rest as training data, evaluating the performance on this subset. We repeat for every subset and finally average the performance over all the experiments.
