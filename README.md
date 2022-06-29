# DemoHash: Hashtag Recommendation based on User Demographic Information

We present the demographic hashtag recommendation DemoHash model to utilize users' demographic information extracted from their selfie images, in addition to textual and visual information. We also propose demographic module to reflect weights betwween co-feature of contents and demographic information. We extended our model based on the [Implementation and dataset of AAAI 2019 paper: Hashtag Recommendation for Photo Sharing Services](https://github.com/SoftWiser-group/MaCon). 

The below figure is the overview of DemoHash; 1) Blue box: post module represents the process of extracting post feature from images and text. 2) Orange box: demographic module represents the process extracting of demographic information and user information feature. 3) Green box: final concatenation of two modules recommends hashtags to users using overall features.

<p align="center">
<img src=https://user-images.githubusercontent.com/96400041/161210421-2ea52f17-3702-4851-98d6-8b3b11fabeb7.png width=45%>
</p>

### Requirements

```
python==3.6
tensorFlow==2.4.1
Keras==2.4.3
```

### Experiment

1. Extracting demographic information(age, gender, race and emotion)
: To extract demographic information from user's selfie images, we use DeepFace library, which is a face recognition and facial attribute analysis framework.

DeepFace's github : https://github.com/serengil/deepface

```
Model/DeepFace.ipynb
```

2. Training and testing DemoHash model
: We train the proposed model using image, text and demographic information. We uploaded only feautre files in order to protect personal information of Instagram users.

```
Model/DemoHash.ipynb
```

Below figures show examples of recommended hashtag results by DemoHash model.

- Examples

<img src=https://user-images.githubusercontent.com/96400041/161210869-ea18cbff-a752-40ff-9825-cb37c789929e.png width=45%> <img src=https://user-images.githubusercontent.com/96400041/161210941-4233c446-aa64-4b02-8622-18d05c175d7f.png width=45%>


### Reference








