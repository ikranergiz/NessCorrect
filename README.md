# The Goal of the NessCorrect
NessCorrect project aims to increase cognitive interaction.

# What is NessCorrect?
*<p align="center">"Estimate hand landmarks and detect mobile phones. Touch the screen when it turns blue."* </p>

<p align="center"><img src="https://github.com/ikranergiz/NessCorrect/blob/main/output%20of%20the%20project.gif" width="450" height="450"/> </p>
<p align="center"><sub>Output of the NessCorrect</sub></p>

This is a program that recognizes hand landmarks using Mediapipe (Python version) and detects mobile phones with a trained YOLOv5 model.

Let's get started by picking up your mobile phone. While holding it, you'll see your detected hand landmarks and mobile phone. If its screen turns blue, it means a blue color-changing signal. Now, you have to touch the mobile phone screen within 5 second. After that, you are going to see the "WELL DONE!" as a message in the left corner of the screen.

This project contains the following topics. 

* Object detection (YOLOv5)
* Signal (Flashing blue) detection (OpenCV-python)
* Hand pose estimation (Mediapipe hands)

# Requirements
* Mediapipe 0.8.1 or later
* OpenCV 4.6.0 or later
* YOLOv5

# Demo
First, you need to clone YOLOv5 repository and install requirements with code below.
```bash
git clone https://github.com/ultralytics/yolov5  # clone
cd yolov5
pip install -r requirements.txt  # install
```
After installing YOLOv5 on your local system, you will be ready to clone this repository.
```bash
git clone https://github.com/ikranergiz/NessCorrect
```
Here's how to run NessCorrect using your webcam.
```bash
python ness_correct.py
```

# Directory
<pre>
│  ness_correct.py
│  Mobile_Phone_Roboflow_Train_YOLOv5.ipynb
|  best.pt
|
├─yolov5
</pre>
## ness_correct.py
This is a main program for inference. 

## Mobile_Phone_Roboflow_Train_YOLOv5.ipynb
This file is a model training script for detecting mobile-phones.

## best.pt
This file was produced with training YOLOv5.

## yolov5
You should clone YOLOv5 repository for creating yolov5 directory.

# Datasets

**Train**
- [Mobile-phones](https://app.roboflow.com/myworkspace-saqaq/mobile-phone/1)

**Test**
- [Mobile-phones](https://app.roboflow.com/myworkspace-saqaq/mobile-phone-test/1)
