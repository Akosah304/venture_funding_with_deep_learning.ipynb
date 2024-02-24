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



## Fig. 1: 

![Fig. 1](https://github.com/toniahurst/FinTech_Module_13/blob/main/Screen%20Shot%202021-09-26%20at%2011.20.51%20PM.png)

## Technologies

This program uses Python 3.7.10, Anaconda version 4.10.3, and JupyterLab 3.0.14. It also uses libraries from Pandas, Keras, and Tensorflow. It was written on macOS Catalina 10.15.7 and run using Google Colab.