# Traffic_Sign_Classification

In this project, I have classified images of German Traffic signs into their 43 different categories using CNN and LeNet model.I built the network on Keras framework running on top of Tensorflow backend, trained on Google Colab using thousands of images in the training set and attained an accuracy of 96.89% against the test set.


# Contents
1. Python Libraries
2. Understanding the dataset
3. Key- points
4. Model Architecture 
5. Training the model
6. Prediction

#  Python Libraries
Open CV

Numpy

Pandas

Matplotlib

Pickle

# Understanding the Dataset
The german traffic signs dataset was used. This dataset has already - split data for training and validation. It has thousands of images of german trafic signs.
https://bitbucket.org/jadslim/german-traffic-signs

# Key-points
Images were made black and white so as to reduce the number of parameters as color is not required to classify traffic signs. 
Histogram Equalizer was used to standardize lighting in all images.
ImageGenerator was used for data augmentation i.e. to produce the images at different angles and views thus strengthening our test data.

# Model Architecture
LeNet model was used

Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_5 (Conv2D)            (None, 28, 28, 60)        1560      
_________________________________________________________________
conv2d_6 (Conv2D)            (None, 24, 24, 60)        90060     
_________________________________________________________________
max_pooling2d_4 (MaxPooling2 (None, 12, 12, 60)        0         
_________________________________________________________________
conv2d_7 (Conv2D)            (None, 10, 10, 30)        16230     
_________________________________________________________________
conv2d_8 (Conv2D)            (None, 8, 8, 30)          8130      
_________________________________________________________________
max_pooling2d_5 (MaxPooling2 (None, 4, 4, 30)          0         
_________________________________________________________________
flatten_2 (Flatten)          (None, 480)               0         
_________________________________________________________________
dense_4 (Dense)              (None, 500)               240500    
_________________________________________________________________
dropout_2 (Dropout)          (None, 500)               0         
_________________________________________________________________
dense_5 (Dense)              (None, 43)                21543     
=================================================================


# Training the model
I trained this model in an online cloud instance on Google Colab.

# Prediction
