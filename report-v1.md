# Report for First Draft of Final Project

### What I did

For my project, I am trying to build a diabetes diagnosis predictor. To do this, I have been playing around with a KNN Classification model, and I will later try a Random Forest model. My data already came with a label signifying whether an individual was diagnosed with diabetes, so I am using that in this supervised learning approach.

Since I would like to focus on capturing individuals who are likely to be diagnosed with diabetes, I wish to optimize my model for higher recall. I noticed, that for higher and higher values of k, where k is the number of neighbors to be considered by the model, my recall seems to increase. I feel like values of k = 49 aren't ideal, but happen to work well on this data set since the data is balanced and each of my two classes have much more data points than the k value I have selected. I split my data into a training and testing set prior to making any changes to my features, like scaling them, so I tried to avoid target leakage and I feel relatively comfortable with the way I went about it. Because of this, I want to opt for a value of k that is less than or equal to 25 that optimizes for recall, however, I will review this decision soon.

I also narrowed down my features from the initial set of columns to a subset of columns based on what I learned from my EDA. Then, I have been comparing the recall results from different subsets of columns of that subset, which has led me to my final set of features for my KNN model.
