# Painter Recognition
The goal of this project is to implement Deep Learning models based on CNN capable of recognizing the author of a painting starting from its characteristics, such as color and style. 

The dataset used for the project has been downloaded from [Kaggle](https://www.kaggle.com/ikarus777/best-artworks-of-all-time). It contains the paintings of 50 international painters, for a total of 8446 paintings. The paintings differ greatly from each other in size, but also in color and style. 

## Method
Different approaches have been tested to achieve the objective: a CNN from scratch and several CNN in Fine Tuning.   
### CNN *from scratch*
The first approach saw the implementation of a simple CNN *from scratch*. As the network has produced poor results, it has been optimized through a Bayesian search of hyper-parameters. For this purpose, it has been used the Python library `keras_tuner`. Once it has been defined a *search space* for the model's hyperparameters, the library allows to find the optimal configuration with respect to a given parameter (validation accuracy or validation loss).

