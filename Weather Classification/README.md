# Weather Classification
## Introduction
Weather classification task is widely used in Satellite Imagery Analysis, for example, to adjust the land cover, or crop product utilization score based on current Weather condition or forecast the future weather on any area by using Computer Vision as one of the input to predict the weather. 
### Dataset
Multi-class weather dataset(MWD) for image classification is a valuable dataset used in the research paper entitled “Multi-class weather recognition from still image using heterogeneous ensemble method”. The dataset provides a platform for outdoor weather analysis by extracting various features for recognizing different weather conditions. you can find dataset [here](https://data.mendeley.com/datasets/4drtyfjtfy/1)

#### Example of trained data
![image](https://user-images.githubusercontent.com/104628789/170413598-2706b518-11d0-4606-b3b8-808ddf43722b.png)
## Model Training
For image classification task, I applied fortransfer learning from pre-trained Deep Residual Networks (ResNet50) to label on weather regconition in the following class,
1.  Shine
2.  Sunrise
3.  Rain
4.  Cloudy

![image](https://user-images.githubusercontent.com/104628789/170415821-ba8c23b0-1dd0-484e-b52d-0bc62333c87c.png)

As a results, the ResNet50 provide an accuracy at 94.6 % in weather classification dataset.
#### Results of Prediction
![image](https://user-images.githubusercontent.com/104628789/170414190-2caf8969-a3a2-4cd4-9d9a-e632d193c1ae.png)

## Notebook
you can find notebook [here](https://github.com/WarintornNawong/Portfolio/blob/main/Weather%20Classification/Weather%20Forecast%20with%20Deep%20learning%20algorithm.ipynb)
