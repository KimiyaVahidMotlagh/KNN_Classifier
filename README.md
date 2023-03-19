# Handwritten-KNN
KNN is a supervised algoritm which determins a data's label, based on the k nearest training examples in the dataset. This algorithm determin the data is more likely to be in a class by the training data most similar to our test data. In this project, we programmed KNN algorithm manually. The main focus of this project was to show how KNN classifies data.

## Table of Contents
- [Dataset Discription & Functions](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#loading-data) <br />
- [Main Functions](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#knn-functions)  <br />
- [Hyperparameter Tuning(K)](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#hyperpatameter-tuningk) <br />
- [Train & Evaluation](https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/README.md#knn) <br />

## Dataset Discription & Functions
- dataset <br/>
The data we are dealing with has 400 points consisting of their x, y, and labels. Our data is shown in the digram bellow:
<tab><tab>![dataset](https://github.com/MohammadJavadArdestani/Medical-Image-Processing-/blob/main/Pictures/train_dataset.png)

- Load & split train and test data <br />
With Pandas, you can read a CSV file and load the points as a dataframe.  For training a KNN model we need both train and test data. We have some data points to predict test dataset labels. 

## Main Functions
- **distance_calculator** <br />
Mechin learning data often are vectors. KNN algorithm searches for similar training data. The most straightforward function to find the neighbors is the Euclidean distance function.<br />
- **K_nearest_neighbour_classifier** <br />
By knowing the distance between two points, K nearest neighbors are the training points with the least distance. This function would find the frequent labels in the neighbors and classify the test data point as the same label.
- **accuracy_calculator** <br />
Because KNN is a supervised algorithm, we have the test labels. The number of corectly classified labels is divided by the total number of data.
- **data_plot** <br />
The plotter will show the train and test data with their class labels in a 2D coordinate diagram. You can set the inputs for both supervised and predicted labels.

## Hyperpatameter tuning(K)<br />
Setting KNN's hyperparameter is commonly achieved by the elbow chart. for each K from 3 to 20, you can check how different the loss will be and then you can pick the best number for tuning in your scenario. For our datapoints K=13 has the least loss. 

## Train and Evaluation
For training the dataset, we have a function to combine previous functions. We set K as input to set the number of naibours and train our model. This function will predict a label for each test data by the end of training. In order to test how much the model predicted correctly, we call the accuracy calculator. Our handwritten KNN predicts over 88 percent of labels correctly.
