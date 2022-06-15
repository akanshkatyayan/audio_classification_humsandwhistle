# Audio Classification on Hums and Whistle Dataset
This project contains 2 use cases: classify if the audio is Hum or Whistle and classify the song from the 8 iconic Hums and Whistle songs.


#**ML Pipeline:**
<img width="995" alt="image" src="https://user-images.githubusercontent.com/35501313/173903360-a06aa020-2844-4cab-b756-0367af9cdb16.png">

# Basic Solution:
The Basic solution on MLEnd Hums and Whistle data in which we are building a machine learning pipeline which can take an input as any of the hum/whistle record of the below 2 songs and identify the song.

1. Potter
2. StarWars

## Feature Extraction:
Feature extraction functions to get another two features for each of our audio files.:

1. **Chromagram**
2. **MFC coefficients (MFCC)**

<img width="949" alt="image" src="https://user-images.githubusercontent.com/35501313/173905436-5732735d-a2fe-42e1-ac39-d34485276fe5.png">

**Plot Chromograms:**
<br>
<img width="789" alt="image" src="https://user-images.githubusercontent.com/35501313/173905565-f1afd9de-2514-4fd4-92a0-ed173945349e.png">

**Plot MFCC:**
<br>
<img width="430" alt="image" src="https://user-images.githubusercontent.com/35501313/173905650-4f8cb50c-d0ac-416b-b612-bd02a6d3c7ee.png">

## Models Result:
<br>
<img width="291" alt="image" src="https://user-images.githubusercontent.com/35501313/173905794-c2f30457-12e1-4203-8854-1ea018e1071e.png">


## Conclusion:
<br>
The LogisticRegression Classifier and MLPClassifier with logistic function resulted in the best performance in the task of classifying Hums and Whistle data into respective classes. Overall accuracy achieved by these clasifiers is 73% and 74% respectively.

Logistic Regression classifier is easy to implement whereas MLPClassifier is powerful in that it achieves appreciable performance especially taking advantage of grid search, to tune each hyperparameter individually.

# Advanced Solution:

The advanced solution on MLEnd Hums and Whistle data. The goal of building this machine learning pipeline is to take all the humming recording for 8 available songs and identify the song for any of the Hum input audio.

1. Potter
2. StarWars
3. Panther
4. Rain
5. Hakuna
6. Mamma
7. Showman
8. Frozen


## Feature Extraction:
<br>
Feature extraction functions to get another two features for each of our audio files.:
1. **Chromagram**
2. **MFC coefficients**
3. **RMS**: Compute root-mean-square (RMS) value for each frame
4. **Zero-Crossing Rate**

**Plot Audio Signal and Spectrogram: Potter Song** 
<br>
![image](https://user-images.githubusercontent.com/35501313/173904367-074cfeaf-a22f-4042-bf9b-822439db5976.png)

**Plot Audio Signal and Spectrogram: Frozen Song** 
<br>
![image](https://user-images.githubusercontent.com/35501313/173904456-af9c0f30-5031-4222-8e96-5f477a1efb33.png)

**Plot MFCC: Potter Song**
<br>
![image](https://user-images.githubusercontent.com/35501313/173904527-8132991d-d23b-4ad9-96de-f42055346152.png)

**Plot MFCC: Frozen Song**
<br>
![image](https://user-images.githubusercontent.com/35501313/173904575-36163857-8b40-4b48-a5a3-a0816b458928.png)

## Models Result
<br>
![image](https://user-images.githubusercontent.com/35501313/173905044-c3dbde68-f11e-4fce-92d2-89c7e4d3e004.png)

## Confusion Matrix:
<br>
![image](https://user-images.githubusercontent.com/35501313/173904955-b0542ea6-4c35-4438-9082-de5c9adadb9b.png)


## Conclusion:
<br>
To conclude the advanced solution of MLEnd Hums and Whistle, We have attempted to classify the Hums audio files to one of the 8 songs. Multiple features from the audio signals were extracted to identify the audio signals accurately. These features were fed to the machine learning classification models with the labelled classes in the training dataset. Performance was evaluated based on precision, recall, f-score and overall accuracy on the unseen data (validation data).

RandomForestClassifier and MLPClassifier worked best in classifying audio files to their actual songs. We have achieved an Overall accuracy of "44%" and 46% respectively in this process. The low accuracy of the model is due to the bad quality of audio files, many of the hums are not recognizable manually and do not follow the same pitch/timeframe of the audio.

Feature extraction and scaling is the most important part of the machine learning piepline and thus needs more in-depth research.
