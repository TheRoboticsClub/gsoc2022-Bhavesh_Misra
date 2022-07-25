---
title: "Coding Period: 7"
excerpt: "Midterm Evaluation (Please don't get kicked xD)"
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

Week 6


## Objectives

- [X] Check the codebase as well 
- [X] Close the ssd_mobilenetv2 model
- [X] Show the running model
- [] Use seaborn to get prettier plots
- [] Updating the graph in real time


## The execution

The first thing that I decided was to close the ssd_mobilenetv2,but decided to use the ssdlite_mobilenetv2 model, as it's apparently just faster that the non-lite model, and then, i went to find a model trained on the coco dataset (no specific reason, just knew that the COCO dataset also covers humans in it's object detection process). And after finding it on the tensorflow object detection site [7], i moved on to convert it to the ONNX format.
Since  I had already done the process for the SSD_volumenetv1, i decided to just reuse that, since both the versions contain the same input and output shapes and dimensions.
So after obtaining the ONNX model, i decided to run the RoboticsAcademy exercise with it, I found out that the this model was getting a better benchmarking score than the previous one (36.2% mAP vs. 35% mAP), which was to be expected, since it's just an upgrade (a higher version) to the previous model. However, the other 3 parts of the exercise didn't work on my model, which I'm pretty sure is a problem in my laptop, a not in the exercise itself.
Next, i went through the codebase as well, by following the Readme [8], as it explained how RoboticsAcademy was built and the interactions between all the different parts work.


## References

[1] [https://github.com/JdeRobot/RoboticsAcademy](https://github.com/JdeRobot/RoboticsAcademy)\\
[2] [https://onnxruntime.ai/](https://onnxruntime.ai/)\\
[3] [https://www.khronos.org/nnef](https://www.khronos.org/nnef)\\
[4] [https://github.com/onnx/models](https://github.com/onnx/models)\\
[5] [https://github.com/KhronosGroup/NNEF-Tools/tree/master/models#nnef-model-zoo](https://github.com/KhronosGroup/NNEF-Tools/tree/master/models#nnef-model-zoo)\\
[6] [https://www.tensorflow.org/tutorials](https://www.tensorflow.org/tutorials)\\ 
[7] [https://github.com/tensorflow/models/tree/master/research/object_detection/models](https://github.com/tensorflow/models/tree/master/research/object_detection/models)\\
[8] [https://github.com/JdeRobot/RoboticsAcademy/blob/master/docs/InstructionsForDevelopers.md](https://github.com/JdeRobot/RoboticsAcademy/blob/master/docs/InstructionsForDevelopers.md)\\