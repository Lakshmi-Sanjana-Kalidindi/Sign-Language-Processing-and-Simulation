
# Sign Language Interpreter using Deep Learning
> A sign language interpreter using live video feed from the camera. 
## Table of contents
* [General info](#general-info)
* [Screenshots](#screenshots)
* [Demo](#demo)
* [Technologies and Tools](#technologies-and-tools)
* [Setup](#setup)
* [Process](#process)
* [Code Examples](#code-examples)
* [Features](#features)
* [Status](#status)
* [Contact](#contact)

## General info

The theme at HACK UNT 19 was to use technology to improve accessibility by finding a creative solution to benefit the lives of those with a disability. 
We wanted to make it easy for 70 million deaf people across the world to be independent of translators for there daily communication needs, so we designed the app to work as a personal translator 24*7 for the deaf people.

## Demo
![Example screenshot](./img/demo4.gif)



![Example screenshot](./img/demo2.gif)



![Example screenshot](./img/demo3.gif)


## Screenshots

![Example screenshot](./img/Capture1.PNG)
![Example screenshot](./img/Capture.PNG)

## Technologies and Tools
* Python 
* TensorFlow
* Keras
* OpenCV

## Setup

* Use comand promt to setup environment by using install_packages.txt and install_packages_gpu.txt files. 
 
`pyton -m pip r install_packages.txt`

This will help you in installing all the libraries required for the project.

## Process

* Run `set_hand_histogram.py` to set the hand histogram for creating gestures. 
* Once you get a good histogram, save it in the code folder,
* Added gestures and label them using OpenCV which uses webcam feed. by running `create_gestures.py` and stores them in a database. A
* Add different variations to the captured gestures by flipping all the images by using `Rotate_images.py`.
* Run `load_images.py` to split all the captured gestures into training, validation and test set. 
* To view all the gestures, run `display_gestures.py` .
* Train the model using Keras by running `cnn_model_train.py`.
* Run `final.py`. This will open up the gesture recognition window which will use your webcam to interpret the trained American Sign Language gestures.  



## Features
Our model was able to predict the 44 characters in the ASL with a prediction accuracy >95%.

Features that can be added:
* Deploy the project on cloud and create an API for using it.
* Increase the vocabulary of our model
* Incorporate feedback mechanism to make the model more robust
* Add more sign languages



