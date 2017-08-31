# Support Vector Machines

Support vector machines (SVMs) are **supervised** learning models with associated learning algorithms that analyze data and recognize patterns, used for classification and regression analysis.

Given a set of training examples, each marked for belonging to one of two categories, an SVM training algorithm builds a model that assigns new examples into one category or the other, making it a non-probabilistic binary linear classifier.

An SVM model is a representation of the examples as points in space, mapped so that the examples of the separate categories are divided by a clear gap that is as wide as possible.

New exmaples are then mapped into that same space and predicted to belong to a category based on which side of the gap they fall on.

However, there can be many options of hyperplanes that separate perfectly, so how do we determine which option to choose?

We would like to choose a hyperplane that maximizes the margin between classes. The vector points that the margin lines touch are known as ***Support Vectors***.

We can expand this idea to non-linearly separable data through the "kernel trick".