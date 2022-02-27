# Image-Classification
### Description
The following performs image classification using Spark Deep Learning Pipelines on the Pokemon Image Kaggle Dataset found here: [https://www.kaggle.com/vishalsubbiah/pokemon-images-and-types](https://www.kaggle.com/vishalsubbiah/pokemon-images-and-types). This program tries to predict the primary type of Pokemon  based on the image. The input dataset was used to sort the input file into the types of primary Pokemon in order to perform the image processing. The output performs the predictions based on the training dataset and prints the evaluation metric of accuracy. My assumption is the accuracy on the test set would be higher based on the maxIters of the LogisticRegression classifier, but Databricks was throwing an OOM issue due to the larger set. Additionally, there was a total of 18 classes that the pokemon could possibly be classified as. 

### How to Run
The Databricks notebook can be accessed at the following URL:
https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1005059527658068/3881870488981072/7740729220923964/latest.html


The input files and relevant files are hosting publicly on s3:
The zip file of sorted Pokemon by primary types: [https://s3.amazonaws.com/cs6350.0u1/Assignment2/primaryPokemonSorted.zip](https://s3.amazonaws.com/cs6350.0u1/Assignment2/primaryPokemonSorted.zip)
The original csv from the Kaggle dataset which included the names 
