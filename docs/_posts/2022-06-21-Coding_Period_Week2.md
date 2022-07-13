---
title: "Coding Period: Week 2"
excerpt: "Continuation of Coding Period- Week 1"
usemathjax: true
sidebar:
  nav: "docs"

toc: true
toc_label: "Contents"
toc_icon: "cog"


categories:
- GSoC
tags:
- Docker
- Virtualenv
- Robotics Academy

author: Bhavesh Misra
pinned: false
---


## Overview

So basically, the first week of the coding period ididn't go as well as planned, and I realised that you need to give MUCHH MORE TIMEE to the work that you are doing, and hence, I decided to work on a remaining task of week 1 for week 2 as well. 
Now, as per the week 2 tasks, I feel that the TensorFlow Object detection one should be easier, as I have TRIED (read Tried, not Worked xD) it before, and it gave me a hugeee headache. But now, i'll be more focused and work on it more.
As per the reading stuff part, that should be easy, but time-consuming, as the only thing that I do is search my errors on StackOverflow.   
Let's see how week 2 goes!

## Objectives

- [X] Read something about Models that are specifically used for human detection
- [] Understand and work on TFOD (TensorFlow Object Detection), and if time permits, learn PyTorch (like atleast be in a position to understand code in PyTorch)
- [X] Convert a model from TensorFlow(Models from TFOD) to ONNX 
- [X] Check the compatibility of both formats for Robotics Academy

## The execution
My thought process was to start reading about the Models that are Specifically used for Human Detetction. Well, across this, I came about the Tiny YOLO model, the SSD_Volumenet model as well as different CNN models such as R_CNN, Faster R_CNN and ShuffleNet as well.

After reading about the different models that are used specifically for Human Detection, I decided to install the TensorFlow Object Detection API. So, I first cloned the Git repository [6] to my directory, and then installed the Protobuffers and the COCO API. This link [7] helped out a lot for this purpose.

The next work was for me to convert a model from the TFOD API to ONNX, and since the models that were picked up for the Human Detection exercise were available in the ONNX Modle Zoo, I didn't do this. It was collectively decided to use the ONNX Model format for the Exercise.

## References 


[1] [https://github.com/JdeRobot/RoboticsAcademy](https://github.com/JdeRobot/RoboticsAcademy)\\
[2] [https://onnxruntime.ai/](https://onnxruntime.ai/)\\
[3] [https://www.khronos.org/nnef](https://www.khronos.org/nnef)\\
[4] [https://github.com/onnx/models](https://github.com/onnx/models)\\
[5] [https://github.com/KhronosGroup/NNEF-Tools/tree/master/models#nnef-model-zoo](https://github.com/KhronosGroup/NNEF-Tools/tree/master/models#nnef-model-zoo)\\
[6] [https://github.com/tensorflow/models] (https://github.com/tensorflow/models)\\
[7] [https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html] (https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html)\\