# Deep-Learning-Binomial-Expansions
This repository contains some research ideas about Binomial Expansions using Deep Learning (convolutional networks)

## Legacy Research

This folder contains some historic work, showing Pascal's triangle built via perceptrons, and convolutions in MATLAB. This was used with junior Data Scientists to explain the concept mainly as a learning exercise / curioisity.

## Main files

- pascal_revisited.ipynb
    this file picks up rom the 'legacy' folder using keras. It creates a pascal_model module, which is reused in the pascal_binomial_expansion main script

- pascal_binomial_expansion.ipynb
    this is the main file in the repo. It is rather long winded, but covers each step in building the full model for binomial expansions. It takes the pascal_model from previous script, makes use of 'exponent arrays' such that correct coefficients are applied.
    Using SymPy

- multiples_of_thirteen.ipynb
    a very basic file showing alternative use of the indexing mechanism. Here, we can supply known multiples of 13 and show that we can 'match' in bound numbers against these

- latex_supervised.ipynb
    this file firstly creates a series of images of latex equations, created using SymPy. These are representative of factored equations which would be suitable for binomial expansion as demonstrated by 'pascal_binomial_expansion.ipynb'. This file contains a simple CNN model, which has 5 concurrent softmax layers to classify the coefficients, exponents and whether coefficients are positive or negative.
    The Dataset may also be found here: https://ieee-dataport.org/keywords/binomial-expansion


## Latex

This is now added to gitignore but contained latex files used to create draft paper. The paper should be available in /pdf form at the top level of the repo

## Data

This folder is in gitignore but will be created when running latex_supervised notebook. It will contain images of equations ready for recognition, demonstrating that we could perform binomial expansion direct from images.

The data has been uploaded here:
https://ieee-dataport.org/keywords/binomial-expansion
