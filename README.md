# Gesture Recognition using DL
An assignment to train a Deep Learning (DL) model to recognize 5 hand gestures correctly when a user does a hand gesture in front of a web camera.

## Table of Contents
* [General Info](#general-information)
* [Project Contents](#project-contents)
* [Conclusion](#conclusion)
* [Software and Library Versions](#software-and-library-versions)
* [Acknowledgements](#acknowledgements)

### General Information
Imagine you are working as a data scientist at a home electronics company which manufactures state of the art smart televisions. You want to develop a cool feature in the smart-TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote.<br>
<br>
The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:<br>
* **0** - Left swipe: 'Jump' backwards 10 seconds
* **1** - Right swipe: 'Jump' forward 10 seconds
* **2** - Stop: Pause the movie
* **3** - Thumbs down: Decrease the volume
* **4** - Thumbs up:  Increase the volume

#### Data Set Brief Information
The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use.<br>
<br>
The data is in a zip file. The zip file contains a 'train' and a 'val' folder with **two CSV files** for the two folders. These folders are in turn divided into subfolders where each subfolder represents a video of a particular gesture. Each subfolder, i.e. a video, contains **30 frames (or images)**. Note that all images in a particular video subfolder have the same dimensions but **different videos may have different dimensions**. Specifically, videos have two types of dimensions - either **360x360** or **120x160** (depending on the webcam used to record the videos).<br>
<br>
Each row of the CSV file represents one video and contains three main pieces of information - the name of the subfolder containing the 30 images of the video, the name of the gesture and the numeric label (between 0-4) of the video.<br>

#### Business Objective
Use different architectures to build a DL model to classify 5 gestures correctly by training the model on the 'train' folder which performs well on the validation 'val' folder as well.

#### Business Solution
The trained model should be fit enough to be used in small web camera and identify the 5 gestures in real-time.


### Project Contents
* **Gesture Recognition Case Study.ipynb** - Jupyter Notebook for Gesture Recognition using DL (Language : Python)
* **Gesture Recognition Write-up.docx** - A docx File for brief explanation of the models designed and its conclusion
* **Gesture Recognition Write-up.pdf** - A pdf File for brief explanation of the models designed and its conclusion
* **model-00017-0.03484-0.98944-0.07473-0.99000.h5** - **Final Trained model** (Model 11) for Gesture Recognition
* model_init_2023-02-1216_13_47.497290 - Folder containing trained model of Model 1
* model_init_2023-02-1218_45_12.635075 - Folder containing trained model of Model 5
* model_init_2023-02-1313_38_00.787330 - Folder containing trained model of Model 10
* model_init_2023-02-1314_06_07.085500 - Folder containing trained model of Model 11
* **README.md** - Readme file


### Conclusion
Any Image classification can be solved using DL.
* **Data Downloading-Unzipping** → Dataset was downloaded from shared drive and unzipped.
* **Data Reading/Data Understanding** → Defined the path for train and validation images.
* **Dataset Creation** → Created train & validation dataset from the train directory with user defined batch size. Also, resized, normalized and cropped images as required.
* **Model Building & training** → Created different DL models for fine tuning the accuracy.

#### Recommendation
Model 11 was chosen to classify 5 gestures.
* Training Accuracy - **98.94** %
* Training Loss - **0.03**
* Validation Accuracy - **99** %
* Validation Loss - **0.07**


### Software and Library Versions
* ![Jupyter Notebook](https://img.shields.io/static/v1?label=Jupyter%20Notebook&message=4.9.2&color=blue&labelColor=grey)

* ![NumPy](https://img.shields.io/static/v1?label=numpy&message=1.21.6&color=blue&labelColor=grey)

* ![Tensorflow](https://img.shields.io/static/v1?label=Tensorflow&message=2.9.2&color=blue&labelColor=grey)

* ![Keras](https://img.shields.io/static/v1?label=Keras&message=2.9.0&color=blue&labelColor=grey)

* ![matplotlib](https://img.shields.io/static/v1?label=matplotlib&message=3.2.2&color=blue&labelColor=grey)

* ![sklearn](https://img.shields.io/static/v1?label=sklearn&message=1.0.2&color=blue&labelColor=grey)

* ![cv2](https://img.shields.io/static/v1?label=sklearn&message=4.7.0&color=blue&labelColor=grey)

* ![skimage](https://img.shields.io/static/v1?label=sklearn&message=0.19.2&color=blue&labelColor=grey)

* ![imageio](https://img.shields.io/static/v1?label=sklearn&message=2.19.3&color=blue&labelColor=grey)


### Acknowledgements
This DL based Gesture Recognition assignment was done as part of [Upgrad](https://www.upgrad.com/ ) - **Master of Science in Machine Learning & Artificial Intelligence** programme.


### Contact
Created by [Sanjeev Surendran](https://github.com/Sanjeev-Surendran)


<!-- ## License -->
<!-- This project is not a open source and sharing the project files is prohibited. -->
