# Command Sound Classification
## Introduction
#### DATASET
**speech command dataset** : An audio dataset of spoken words designed to help train and evaluate keyword spotting systems. Its primary goal is to provide a way to build and test small models that detect when a single word is spoken, from a set of ten target words, with as few false positives as possible from background noise or unrelated speech. Note that in the train and validation set, the label "unknown" is much more prevalent than the labels of the target words or background noise. One difference from the release version is the handling of silent segments. While in the test set the silence segments are regular 1 second files, in the training they are provided as long segments under "background_noise" folder. Here we split these background noise into 1 second clips, and also keep one of the files for the validation set. you can find data set [here](http://storage.googleapis.com/download.tensorflow.org/data/mini_speech_commands.zip)

## Key Findings
#### 5 Example of Wave form and Spectrogrma of "UP" command
![image](https://user-images.githubusercontent.com/104628789/170480583-ae10e1d2-008f-4b25-8039-ab371e4a2380.png)

#### 5 Example of Wave form and Spectrogrma of "DOWN" command
![image](https://user-images.githubusercontent.com/104628789/170480634-97d8713d-6e16-436b-a2c8-9aa2b3d2fd64.png)

#### 5 Example of Wave form and Spectrogrma of "LEFT" command
![image](https://user-images.githubusercontent.com/104628789/170480721-bc7786fc-b266-41f3-aa8b-fa739c9fae85.png)

#### 5 Example of Wave form and Spectrogrma of "RIGHT" command
![image](https://user-images.githubusercontent.com/104628789/170480758-f2d3221a-372b-4410-98e7-8a1322702d13.png)

#### 5 Example of Wave form and Spectrogrma of "GO" command
![image](https://user-images.githubusercontent.com/104628789/170480792-93533e1f-86a1-4b6f-a85e-94c986ee7023.png)

#### 5 Example of Wave form and Spectrogrma of "STOP" command
![image](https://user-images.githubusercontent.com/104628789/170480834-f230b356-04a7-491c-9bd2-61befd0f1bcd.png)

#### 5 Example of Wave form and Spectrogrma of "YES" command
![image](https://user-images.githubusercontent.com/104628789/170480875-b27c8da6-ff87-4a97-af92-038c4b4d252c.png)

#### 5 Example of Wave form and Spectrogrma of "NO" command
![image](https://user-images.githubusercontent.com/104628789/170480953-aa3bf0aa-60a0-4a2d-8852-2574808c5ba5.png)

####  Example of Wave form and Spectrogrma of All command
![image](https://user-images.githubusercontent.com/104628789/170481090-a0be1b7b-9c05-4ba6-b7e3-80345712152b.png)

### All Command Distribution
![image](https://user-images.githubusercontent.com/104628789/170481221-7f2cc45f-ff50-4cb9-802b-3b8ee8c58262.png)

## Model Constructing
I applied the CNN to classify and differentiate between thier command. Firstly, I set the baseline as simple CNN with the following architechture,


![image](https://user-images.githubusercontent.com/104628789/170481675-6c53ef6d-7f81-4a70-b806-d499f9d4e1a7.png)

- Results



![image](https://user-images.githubusercontent.com/104628789/170482342-9e5ae900-72c5-4cb6-9ae7-ab92bb41afda.png)


and then, I would like to gradually increase a model complexity in the sixth attempt below,
### FIRST ATTEMPTs (Baseline + one CNN layers)

- Results


![image](https://user-images.githubusercontent.com/104628789/170482392-e2905df7-4959-45d7-94b7-b9f9bad0736d.png)

### SECOND ATTEMPTS (Baseline + OneCNN/MaxPool Layers)
- Results

![image](https://user-images.githubusercontent.com/104628789/170482500-8df009a4-2382-4f4d-9b20-ecbe5a6be516.png)

### THIRD ATTEMPTS (Baseline + One Layers+L2)
- Results


![image](https://user-images.githubusercontent.com/104628789/170482565-de06d2e9-c51f-4f0d-bdeb-9da2c9d48f73.png)

### FORTH  ATTEMPTs (Baseline + One CNN + Dropout)
- Results


![image](https://user-images.githubusercontent.com/104628789/170482640-45b7f6e3-ad94-4406-934b-1db1050cf1a8.png)

### FIFTH ATTEMPTS (Baseline + Two CNN Layers + Dropout)
- Results


![image](https://user-images.githubusercontent.com/104628789/170482742-211e9035-2234-4ccd-b049-91dddd6123d4.png)

### SIXTH ATTEMPTS (Baeline + 4 CNN Layers + Dropout)
- Results


![image](https://user-images.githubusercontent.com/104628789/170482811-ad956c7e-8171-4a8e-bba3-31eacea24432.png)



