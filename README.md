# IMPROVED EARLY  CLASSIFICATION OF STREAMING MUSIC USING SVM

## Getting Started

The main objective of our project is to create a model which is able to classify music tracks into two categories i.e. dance and non-dance with a high amount of accuracy and in the minimum duration possible.In the proposed approach, frame-wise classification is done on the data so that even the minute details of an audio are not ignored and we can detect the category as early as possible. Various factors which influence our research like different frame sizes and different set of features are analyzed and their classification accuracy is verified. SVM classifier has been used for our project.



### Prerequisites

To use this work on your researches or projects you need:

Python packages:

* **IPython**

* **Numpy**

* **Scipy**

* **Pandas**

* **Scikit-learn**

* **Librosa**

* **Matplotlib**

* **Pydub**
* **Shutil**
* **Os**
* **Csv**

Jupyter Notebook (with IPython kernel)

### Data Sets

There are two datasets used in this project. Basic experiments were performed using the GTZAN dataset. A brief of the data set:
* **This dataset was used for the well known paper in genre classification " Musical genre classification of audio signals " by G. Tzanetakis and P. Cook in IEEE Transactions on Audio and Speech Processing 2002.**
* **The files were collected in 2000-2001 from a variety of sources including personal CDs, radio, microphone recordings, in order to represent a variety of recording conditions.**
* **The dataset consists of 1000 audio tracks each 30 seconds long. It contains 10 genres, each represented by 100 tracks. The tracks are all 22050Hz Mono 16-bit audio files in .wav format.**
* **Official web-page: marsyas.info**
* **Download size: Approximately 1.2GB**
The genre rock was used from this dataset and another folder non-rock was created by using 11 songs each from the rest of the genres to perform binary rock verse non rock classification.
Since the files in the dataset are in the au format, which is lossy because of compression, they need to be converted in the wav format (which is lossless) before we proceed further.

The second dataset is our self-created dataset created from our own music library. A brief of the dataset :
* **There are two folders named as dance and non-dance and they contain 200 songs each.**
* **The duration of the tracks is 30 seconds each.**


## Code

Documentation
* **STEP 1 - Conversion.py: USAGE: This code is used to convert the audio files from .au and .mp3 to .wav format.**
* **STEP 2 - Framing and FeatureExtraction.py: USAGE: This code is used to extract the required features from the audio files frame-wise and also for writing those features into a csv file.**
* **STEP 3 - Classification.py: USAGE: This code is used to load the csv file, split it into train and test sets and applying svm classifier on it. The trained model is then used for predicting the output of the test set. At last, majority voting is applied on audio tracks one by one to check the result of a particular track frame-wise.**



## Versioning

Python 3.6.3


### Authors
* **Ridhi Sharma**
* **Urvi Fotedar**

## Acknowledgments

* Thanks to DIC,UIET, Panjab University

