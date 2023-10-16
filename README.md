# Data Challenge: Breaking classifiers

The goal of this assignment is to build datasets that is hard for one classifier, but easy for another.  Specifically:

- Pick any two of the six classifiers we've covered (Logistic regression, SGD Classifier, Decision Tree, Naive Bayes, SVM, KNN). Let's call these A & B.
- Build one dataset that A does well on and B does poorly on.
- Build another dataset that B does well on but not A.

In all cases, you should assess performance via F1-score using a 5-fold classifier. You should strive to achieve a difference of at least .02 in average F1-score. 

You might find it useful to examine the [sklearn dataset generators](https://scikit-learn.org/stable/datasets/sample_generators.html) functions.

## Rules

1. You cannot use feature manipulation to cause a classifier to fail - e.g., decision trees are robust to label-encoded data and insensitive to scaling; KNNs are highly sensitive to both.  You must encode your data in a manner that gives both algorithms the best chance they have to do well.
2. For a given dataset, any imputation / pre-processing must be identical across your algorithms.
3. You must submit both the code and the datasets (as csvs).  Please use a "seed" value to ensure reproducibility. 

## Rubric (50 points max).
1. Did you follow the rules?  If not, your assignment will not be accepted.
2. Is your code well organized and clear? (10 pts).
3. Did you achieve at least a .02 difference? (If so, 40 pts.  If not, read on).
4. Did you try several different approaches? Did you include rationale that explains your choices?  Is this rationale correct given what we've learned thus far?

## Extra credit (4 points max).
1. For every .05 point difference in your maximally discrepant results, you will receive a point of extra credit.  That is, if you logistic regression performs a .86 and your decision tree at .92 on dataset A, you would receive 1 point of extra credit. 


