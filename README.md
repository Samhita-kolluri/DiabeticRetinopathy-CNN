# DiabeticRetinopathy-CNN
A model for detecting diabetic retinopathy using cnn

## 1. Setting an Environment:
The environment required for the implementation has to be setup before building the model. This includes importing and installing all the necessary packages and libraries.

## 2. Loading Data and Exploratory Data Analysis :
Fundus data acquisition : Kaggle dataset has 17,563 images.The very first item analyzed was the training labels. While there are five categories to predict against. The classifications in the network are defined numerically as:	
0 - No DR,  1 - Mild DR, 2 - Moderate DR,  3 - Severe DR,  4 - Proliferative DR.

## 3. Preprocessing the Data :
To preprocess the data the images are supposed to be cropped and resized. All images were scaled down to 256 by 256. Despite taking longer to train, the detail present in photos of this size is much greater than at 128 by 128. A matrix is used to store all flattened images.

## 4. Model parameters:
The model  parameter is a configuration variable that is internal to the model and whose value can be estimated from data. These are required by the model when making predictions. These values define the skill of the model. 

## 5. Splitting the Train and Test Data :
Splitting the data into training and testing sets before training the model. The 17,563 images are divided into train and testing data samples 14050 are train samples and 3513 are test samples. Random_state is used for initialing the internal random number generator which will split the data in train and test indices. 

## 6. Model :
For predicting two categories, the model utilizes three convolutional layers, each having a depth of 32. A Max Pooling layer is applied after all three convolutional layers with size (2,2). After pooling, the data is fed through a single dense layer of size 128, and finally to the output layer, consisting of 5 last dense layers.

## 7. Model Evaluation :
After validating our model on a dataset of 17,563 fundus images. Our model was tested and the model was evaluated with 97.1% 
