DU-VIRT-AI-PT-05-2024-U-LOLC-MWTH - Module 13 Challenge (Aug 10, 2024)

# Module 13 Challenge: Supervised Learning - Classification

[notebooks/spam_detector.ipynb](https://github.com/JimGile/classification-challenge/blob/main/notebooks/spam_detector.ipynb)

## Focus

Module 13 focuses on the supervised machine learning concept of clustering
which is used to predict categorical classes based on their distinct features.
It starts with straightforward linear models such as logistic regression and
progresses to more intricate nonlinear models and ensemble methods.

Supervised clustering algorithms and concepts explored in this challenge:

### Linear Classification Models

Linear classification models are fast and work well with data that can be split linearly.
The goal of a linear classifier is to find a line that separates two groups of data.
However, many possible lines might exist, with each creating a different boundary.

* **LogisticRegression**: Despite its name, the Logistic Regession model is implemented
as a linear model for classification rather than regression in terms of the scikit-learn/ML nomenclature. The logistic regression is also known in the literature as logit regression, maximum-entropy classification (MaxEnt) or the log-linear classifier. It expects a categorical target, making the Logistic Regression a classifier. It can fit binary, One-vs-Rest, or multinomial logistic regression.

* **SVC**: C-Support Vector Classification. It implements the support vector machine (**SVM**) algorithm which tries to find a hyperplane that maximizes the boundaries between groups. Hyperplanes are decision boundaries in data spaces that are “flat.”

### Non-Linear Classification Models

Non-Linear classification models are more exhaustive work better with data that is more complex.

* **KNN**: k-Nearest Neighbor model compares known data points to determine
the classification of a novel data point (aka Friendly Neighbor). The k-value parameter tells the algorithm to find the k-number of closest known data points. Then, the algorithm determines what the majority of surrounding data points are classified as to determine the class of the new data point.

* **Decision Trees**: Trees are a family of supervised learning models that provide an alternative to logistic regression and SVMs. They use Root, Branch, and Leaf strategy concepts.

* **Ensemble Learning**: Ensemble learning starts with the idea that two is better than one. A single decision tree might be prone to errors, but many of them can be combined to form a stronger model.

  * **RandomForest**: The random forest model combines many decision trees into a forest of trees.
  * **ExtremelyRandomTrees** (or ExtraTrees) is a similar to random forests. Random forests resample the data for each new decision tree, but extremely random trees reuse the entire sample each time.

## Challenge

The challenge is you work at an Internet Service Provider (ISP) and you've been tasked with improving the email filtering system for its customers. You've been provided with a dataset that contains information about emails, with two possible classifications: spam and not spam. The ISP wants you to take this dataset and develop a supervised machine learning (ML) model that will accurately detect spam emails so it can filter them out of its customers' inboxes.

## Solution

The solution is in the Jupyter Notebook file [notebooks/spam_detector.ipynb](https://github.com/JimGile/classification-challenge/blob/main/notebooks/spam_detector.ipynb).
