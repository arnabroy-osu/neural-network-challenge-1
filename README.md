## Title
Module 18 Neural Network Challenge 1

## Source Data
Data is sourced from EDX AI Library, located at [https://static.bc-edx.com/ai/ail-v-1-0/m18/lms/datasets/student-loans.csvLinks]. The dataset contains 11 features and 1 target variable (credit_ranking), which is the last column in the dataset.

## Desired Outcome of the exercise
The goal of this exercise is make use of our knowledge of TensorFlow to design a deep neural network model using the dataset’s features. We are required to create and fit the model to predict the credit quality of a student. We will need to consider the number of inputs before determining the number of layers and number of neurons on each layer. Finally, we will compile and fit the model and calculate the loss and accuracy. I have also used the Kerastuner library to tune the hyperparameters of the model to improve its performance.

## Dependencies
I have used the following libraries in this exercise:
- pandas
- tensorflow
- sklearn
- pathlib

## Implementation Summary
The dataset was splitted and split into features and target variables & then splitted into training and testing datasets. The features were scaled using the StandardScaler. The deep neural network model was designed using TensorFlow and the model was compiled and fitted. The model was then evaluated using the testing dataset and was optimized using the Kerastuner library to tune the hyperparameters of the model to improve its performance. Next I have saved the model as .keras file and later on loaded the model and did the predictions on the testing dataset. Finally I created the classification report to evaluate the model's performance.

## Use of Google Colab
Initially I have worked this exercise in Google Colab to leverage the GPU for faster processing, saving the model and loading from Colab. But I have to transfer the code to the local machine in  Visual Studio Code to use the Kerastuner library as it was not available in Google Colab, saved the best tuned model in local machine and loaded the model from local machine to do the predictions.