# DogsBreedClassification


## Project Overview

In this project, I built and trained a neural network model with CNN (Convolutional Neural Networks) using transfer learning technique, with a dataset of 8351 dog images of 133 breeds. 


## Installation

* opencv-python==3.2.0.6
* h5py==2.6.0
* matplotlib==2.0.0
* numpy==1.12.0
* scipy==0.18.1
* tqdm==4.11.2
* scikit-learn==0.18.1
* keras==2.0.2
* tensorflow==1.0.0 


## File Descriptions

Below are main foleders/files for this project:
1. haarcascades
    - haarcascade_frontalface_alt.xml:  a pre-trained face detector provided by OpenCV
2. bottleneck_features
    - DogVGG19Data.npz: pre-computed the bottleneck features for VGG-19 using dog image data including training, validation, and test
    - DogVGG16Data.npz: pre-computed the bottleneck features for VGG-16 using dog image data including training, validation, and test
3. saved_models
    - weights.best.VGG16.hdf5: saved model weights with best validation loss using VGG16
    - weights.best.VGG19.hdf5: saved model weights with best validation loss using VGG19
    - weights.best.from_scratch.hdf5: saved model weights with best validation loss building from scratch
4. dog_app.ipynb: a notebook used to build and train the dog breeds classification model 
5. extract_bottleneck_features.py: functions to compute bottleneck features given a tensor converted from an image
6. images: a few images to test the model manually

Note: 
The dog image dataset used by this project can be downloaded here: https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip
The human image dataset can be downloaded here: https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip


## Results

1. The model was able to reach an accuracy of 71.89% on test data.
2. If a dog image is supplied, the model gives a prediction of the dog breed.
3. The model is also able to identify the most resembling dog breed of a person.

Project files can be found in this github repo: https://github.com/PC271199/Capstone
More discussions can be found in this blog: https://medium.com/@phuoccong99/dog-breeds-classification-with-cnn-transfer-learning-2be15cf267eb


## Licensing, Authors, Acknowledgements

Credits must be given to Udacity for the starter codes and data images used by this project. 
