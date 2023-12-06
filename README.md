
# Emotion Detection

This project uses OpenCV and a self trained Keras model to perform real-time emotion detection from webcam video.

## Overview

-   Detects faces in each video frame using Haar Cascades
-   Extracts the detected face regions
-   Resizes face crops to 48x48
-   Normalizes pixel values
-   Passes face crops through model to classify emotion
-   Displays emotion label and bounding box overlay on video

## Usage

To run emotion detection:

    python main.py

A webcam window will open and display the detected emotional state for each recognized face.

## Model

The emotion classifier model is a pre-trained Keras deep learning model (`model.h5`) using the FER-2013 dataset.

It detects the following emotional categories:

-   Angry
-   Disgust
-   Fear
-   Happy
-   Neutral
-   Sad
-   Surprise

## Installation

This project was built with Python 3 and OpenCV. Key dependencies:

 1. opencv-python 
 2.  numpy  
 3. tensorflow

Use pip to install:

    pip install opencv-python numpy tensorflow

## Customization

Some ideas for extending this:

-   Apply recognition to video files or image datasets
-   Retrain model on new dataset for improved accuracy
-   Add additional emotion categories
-   Run recognition on live video streams
-   Build interface to captured emotion analytics over time
## License

MIT license, free for public use and contributions.
Let me know if any other sections would be helpful to include!
