# Handwritten-KNN
KNN is a supervised algoritm which determins a data's label, based on the k nearest training examples in the dataset. This algorithm determin the data is more likely to be in a class by the training data most similar to our test data.

## Table of Contents
- [KNN functions](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#knn-functions)  <br />
- [Loading data](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#loading-data) <br />
- [Hyperparameter tuning(K)](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#hyperpatameter-tuningk) <br />
- [KNN excution and accuracy](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#knn) <br />
## KNN functions
- **distance_calculator** <br />
Often Mechin learning data is defined by vectors. KNN algorithm searches for similar training data. The most straightforward function to find the neighbors is the 2D distance function.<br />
- **K_nearest_neighbour_classifier** <br />
By knowing the distance between two points, K nearest neighbors are the training points with the least distance. This function would find the most labels in the neighbors and classify the test data point as the same label.
- **accuracy_calculator** <br />
Because KNN is a supervised algorithm, we have the test labels. The number of rightly classified labels is divided by the total number of data.
- **data_plot** <br />
The plotter will show the train and test data with their class labels in a 2D coordinate diagram. You can set the inputs for both supervised and predicted labels.

## Loading data
- Read CSV file <br />
With Pandas, you can read a CSV file and load the points as a dataframe. The data we are dealing with is a simple 400 points consisting of their X, Y, and labels.
- split train and test data <br />
For training a KNN model we need both train and test data. We have some data points to predict test dataset labels. 

## Hyperpatameter tuning(K)<br />
Setting KNN's hyperparameter is commonly achieved by the elbow chart. for each K from 3 to 20, you can check how different the loss will be and then you can pick the best number for tuning in your scenario. For our datapoints K=13 has the least loss. 

## KNN train and evaluation
For training the dataset, we have a function to combine previous functions. We set K as input to set the number of naibours and train our model. This function will predict a label for each test data by the end of training. In order to test how much the model predicted correctly, we call the accuracy calculator. Our handwritten KNN predicts over 88 percent of labels correctly.
