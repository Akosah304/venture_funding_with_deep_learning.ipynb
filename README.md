# FinTech_Module_13 Challenge

# Background

In this challenge, we posed as a risk management associate at Alphabet Soup, a venture capital firm. The team has asked you to help them create a model that predicts whether applicants will be successful if funded by Alphabet Soup. To make the evaluation, we were given a CSV file containing more than 34,000 organizations that have received funding from Alphabet Soup. The CSV file provides information on each business, including whether or not it ultimately became successful. Our challenge was to apply machine learning and neural networks to create a binary classifier model to predict whether an applicant will become a successful business.

## Purpose:

The goal of this project is to optimize a neural network for a start-up success-related binary classification problem. 

Funding applications that are sent to different incubators or venture capital firms should pass through the model as a filter. That specific company might be a wise choice for investment if the model accurately forecasts startup success.

## Approach:

I tested eight different models in addition to my initial model, which achieved a respectable degree of accuracy and a manageable loss rate. I varied the number of epochs used to train the models, the activation function, the layer number, and the number of neurons in each hidden layer. 

Surprisingly, my original model ended up being the best choice in terms of accuracy and loss minimization. 

In terms of model performance, Alternative model 7 is the closest rival. I increased the epoch size to 300 and added an extra hidden layer to alternative model 7, which had a structure and activation functions identical to the original model. Compared to my initial attempt, the outcomes were still marginally less optimal.

## Results:

Of the eight models examined for this study, the original model has the best predictive power for startup success. This should serve as a standard for any future model generation rather than preventing any more optimization attempts. 

## Technologies

This program uses Python 3.7.10, Anaconda version 4.10.3, and JupyterLab 3.0.14. It also uses libraries from Pandas, Keras, and Tensorflow. It was written on macOS Catalina 10.15.7 and run using Google Colab.

## Instructions
The instructions for this Challenge are divided into the following subsections:

* Prepare the Data for Use on a Neural Network Model

* Compile and Evaluate a Binary Classification Model Using a Neural Network

* Optimize the Neural Network Model

## Prepare the Data for Use on a Neural Network Model
Using your knowledge of Pandas and StandardScaler from scikit-learn, preprocess the dataset so that you can later use it to compile and evaluate the neural network model. To do so, complete the following steps:

- Read the applicants_data.csv file into a Pandas DataFrame. Review the DataFrame, checking for categorical variables that will need to be encoded and for columns that might eventually define your features and target variables.

- Drop the “EIN” (Employer Identification Number) and “NAME” columns from the DataFrame, because they’re irrelevant for the binary classification model.

- Encode the categorical variables of the dataset by using OneHotEncoder, and then place the encoded variables in a new DataFrame.

- Add the numerical variables of the original DataFrame to the DataFrame that contains the encoded variables

## NOTE
To complete this step, use the Pandas concat function.

Using the preprocessed data, create the features (X) and target (y) datasets. The “IS_SUCCESSFUL” column in the preprocessed DataFrame should define the target dataset. The remaining columns should define the features dataset.

- Split the features and target datasets into training and testing datasets.

- Use StandardScaler from scikit-learn to scale the features data.

## Compile and Evaluate a Binary Classification Model Using a Neural Network
Use your knowledge of TensorFlow to design a binary classification deep neural network model. This model should use the features of the dataset to predict whether a startup that’s funded by Alphabet Soup will become successful. Consider the number of inputs before determining both the number of layers that your model will contain and the number of neurons on each layer. Then compile and fit your model. Finally, evaluate your binary classification model to calculate the model’s loss and accuracy.

To do so, complete the following steps:

1. Use Tensorflow’s Keras to create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer.

2. Compile and fit the model by using the binary_crossentropy loss function, the adam optimizer, and the accuracy evaluation metric

3. Save and export your model to an HDF5 file, and name the file AlphabetSoup.h5.

## Optimize the Neural Network Model
Using your knowledge of TensorFlow and Keras, optimize your model to improve its accuracy. Even if you don’t achieve a better accuracy, you'll need to demonstrate at least two attempts to optimize the model. You can include these attempts in your existing notebook. Or, you can make copies of the starter notebook in the same folder, rename them, and code each model optimization in a new notebook.

## NOTE
You won’t lose points if your model doesn’t achieve a high accuracy—as long as you make at least two attempts to optimize the model.

To do so, complete the following steps:

* Define at least three new deep neural network models (that is, the original plus two optimization attempts). For each, try to improve your first model’s predictive accuracy.

* Display the accuracy scores that each model achieved, and then compare the results.

* Save each model as an HDF5 file.
