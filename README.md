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
A modified version of the LeNet model was used.
![model_arch](https://user-images.githubusercontent.com/55614154/122716871-724d8400-d288-11eb-9c8c-44a5babd135e.png)



# Training the model
I trained this model in an online cloud instance on Google Colab over 30 epochs.

# Prediction

The model achieved 95.7% accuracy.


![Model_loss](https://user-images.githubusercontent.com/55614154/122716854-6c57a300-d288-11eb-978e-d1d4fb67ae1b.png)


![Model_accuracy](https://user-images.githubusercontent.com/55614154/122716862-6eb9fd00-d288-11eb-9519-f1f56c004631.png)


