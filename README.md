# Animal-Breed-Classification-using-CNN


## Table of Content
  * [Problem_Definition](#Problem_Definition)
  * [Dataset_Description](#Dataset_Description)
  * [Model_Building](#Model_Building)
  * [Result](#Result)
  * [Model Deployment ](#Model_Deployment )
  * [Credit](#Credit)
  

 
 ## Problem_Definition
 One the objective of the project is to predict the breed of a dog and cat using its image. 
The Convolutional Neural Network model that I will make, will be classifying an animal breed among 37 different breeds of dog and cat based on its processing of the image and classify it to the appropriate breed. In the end, the CNN model should predict the top3 breed with the probability of breed based on its image .

 ## Dataset_Description
 
Dataset Link:  [Animal_Breed](https:// https://dockship.io/challenges/5fdcba715f392d4d66289d43/animal-breed-classification-ai-challenge/overview)

The dataset contains images of 37 breeds of cats and dogs from around the world. It contains two directories "TRAIN" and "TEST" with 5890 and 1500 images respectively. The training images are provided in the directory of the specific class itself. The names of the directories are "class labels" to be used for submission. The aim is to classify the "TEST" images into one of the 37 classes.




## Model_Building
*  I followed the following steps to build a Convolutional neural network-
1.	Import Required library
2.	Initialize CNN and add a convolutional layer
3.	Pooling
4.	Similarly, add two more convolutional layer
5.	Flattening operation
6.	Fully connected layer & output layer

     

## Result
* Testing the model on some animal breed 2015 to check how it’s performing.
* The predicted top 3 breeds for the following images are below: 
       * English_setter
       * 
       <img src="/english_setter.png" width="300">
       
       Prediction-  1. english_setter
                    2. yorkshire_terrier
                    3. shiba_inu


       

       

## Model Deployment 
* Deployed dmodle using **GRADIO library.

[deploymodel_videolink](https://drive.google.com/file/d/1EvX9K8XDGWYgAEHhgv6xP9AjglNuY0z0/view?usp=sharing) 

## Credit
[dockship](https://dockship.io/challenges/5fdcba715f392d4d66289d43/animal-breed-classification-ai-challenge/overview) - This project has been done on this competitive platform.

