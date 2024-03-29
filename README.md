# KNN_Classifier
KNN is a supervised algorithm that determines a data's label, based on the k nearest training examples in the dataset. This algorithm determines the data is more likely to be in a class by the training data most similar to our test data. In this project, we programmed the KNN algorithm manually. The main focus of this project was to show how KNN classifies data.

## Table of Contents
- [Dataset Description & Functions](https://github.com/KimiyaVahidMotlagh/KNN_Classifier#dataset-discription--functions) <br />
- [Main Functions](https://github.com/KimiyaVahidMotlagh/KNN_Classifier/blob/main/README.md#main-functions)  <br />
- [Hyperparameter Tuning(K)](https://github.com/KimiyaVahidMotlagh/KNN_Classifier#hyperpatameter-tuningk) <br />
- [Train & Evaluation](https://github.com/KimiyaVahidMotlagh/KNN_Classifier/blob/main/README.md#train-and-evaluation) <br />

## Dataset Discription & Functions
- dataset <br/>
The data we are dealing with has 400 points consisting of their x, y, and labels. Every class in the dataset is shown in a different color. Each point has a corresponding label to separate the classes. <br/> Our data is shown in the diagram below: <br/><br/>

<picture>
 <source media="(prefers-color-scheme: dark)" srcset="https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/Pictures/dataDarkmode.jpg">
 <img alt="Shows an illustrated sun in light color mode and a moon with stars in dark color mode." src="https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/Pictures/Data.jpg">
</picture> <br/>

- Load & split train and test data <br />
With Pandas, you can read a CSV file and load the dataset as a dataframe. For training a KNN model we need both train and test data. We have some data to predict test dataset labels and then evaluate our code. To achieve that we used Scikit Learn's split data function.

## Main Functions
- **distance_calculator()** <br />
Machine learning data consists of vectors. KNN algorithm searches for similar training data. The most straightforward function to find the neighbors is the Euclidean distance function.<br />
- **K_nearest_neighbour_classifier()** <br />
By knowing the distance between two points, K nearest neighbors are the training points with the least distance. This function would find the frequent labels in the neighbors and classify the test data point as the same label.
- **accuracy_calculator()** <br />
Because KNN is a supervised algorithm, we have the test labels. The number of correctly classified labels is divided by the total number of data.
- **data_plot()** <br />
The plotter will show the train and test data with their class labels in a 2D coordinate diagram. You can set the inputs for both supervised and predicted labels.

## Hyperpatameter Tuning(K)<br />
Setting KNN's hyperparameter is commonly achieved by the elbow chart. For each K from 3 to 20, you can check how different the loss will be and then you can pick the best number for tuning in your scenario. <br/>

<picture>
 <source media="(prefers-color-scheme: dark)" srcset="https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/Pictures/elbowDarkmode.jpg">
 <img alt="Shows an illustrated sun in light color mode and a moon with stars in dark color mode." src="https://github.com/KimiyaVahidMotlagh/Handwritten-KNN/blob/main/Pictures/elbow.jpg">
</picture>

For our dataset, K=13 has the least loss. 

## Train and Evaluation
For training the dataset, we have a function to combine previously mentioned functions. We set K as input to set the number of naibours and train our model. This function will predict a label for each test datapoint by the end of training. To test how much the model predicted correctly, we call the accuracy calculator. Our KNN predicts over 88 percent of labels correctly.
