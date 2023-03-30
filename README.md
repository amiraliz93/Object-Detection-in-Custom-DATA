# Object-Detection-in-Custom-DATA (AI Application For People with Visually impaired)
Aim of this project:
With the aid of artificial intelligence, a mobile app was designed and put into use to help those with visual impairments find a safe place to cross the street more conveniently.
1- This is a Android based project to able visually impaired people to be more independent in crossing street by detecting the three main sign Traffic-light, crossing-sign and zebra line.
You can see the orginal code on Colab with Link:
## Colab https://colab.research.google.com/drive/17fzlTLqk5OE6KfRAu5upsjAo1M3M_3x3?usp=sharing

# ROADMAP TO CREATING AN OBJECT DETECTION TFLITE MODEL
- Collect the dataset of images and label them to get their xml files.

- Augmente and develope our detaset to increase our model accuracy

- Install the TensorFlow Object Detection API.

- Generate the TFRecord files required for training. (need generate_tfrecord.py script and csv files for this)

- provide pre-train models and train them by my dataset.

- Train and evaluate the model.

- using tensorboard to follow the training processes

- Export and convert the model into TFlite(TensorFlow Lite) format.

- Deploy the TFlite model on Android / iOS / IoT devices.

**Model**
- In this project, different EfficientDet models and ssd_Mobilenet are used and compared to reach efficient model.
  The performance of models displayed on the below Table.
- Although the speed of the model slows down as its complexity rises, by increasing its complexity, 
models may describe spatial linkages in the form of folds and hence perform better. All model 
trained with these parameters: epochs:200, epoch size: 8
![1](https://user-images.githubusercontent.com/63164352/193473298-52f37bbc-ac13-453d-a076-9e3ec7e73fcd.PNG)

**Final Model**
I chose the lightest model, EfficientDet-Lite0, after analyzing and testing other models, taking 
into account the various elements that may be altered for each model in order to speed up 
identification and minimise calculations.
Also, I set the number of epochs as high as possible by 
considering validation error in order to increase the model accuracy and the final epoch number 
and batch size considered for this model were 1000 and 8 respectively.
![3](https://user-images.githubusercontent.com/63164352/193474518-15702cac-d2e3-4dda-a040-7bb5b0604941.PNG)

# Finall App



https://user-images.githubusercontent.com/63164352/228875297-8abc5c2c-af54-4c96-b9a5-eb00e91b54a2.mp4



Full videos: 
https://www.youtube.com/shorts/OSQLTR0knLI


# Notice
- The dataset can download from ImageData by using the get_data file
- Visually_impaired, Model_maker and ModelE1_Epoch1000_B8 files are the training model and for final app the trained model of ModelE1_Epoch1000_B8 was used
- THE FINAL app named Detection and can be find here
