---
title: "Coding Period: Week 1"
excerpt: "Identify, resolve issues and add features in main tools"
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

So basically, the first week of the coding period is understanding the different formats that are available to represent Machine learning models, and to understand them. Currently, Robotics Academy[1] uses the ONNX[2] format to do this work, however, my work is to understand the ONNX and the NNEF[3] formats.

Soo, in order to carry out the Objectives, I plan to use the ONNX Model Zoo[4] and the NNEF model Zoo[5] to compare the speeds of the models in general, and then, if time permits, try running them for the Robotics Academy- Deep Learning HUman Detection exercise. 
I have worked with TensorFlow before, but not with Pytorch. Hence, I plan to understand the Pytorch framework as well, to carry out the final objective.


## Objectives

- [X] Compare the same models in ONNX and NNEF formats in terms of time and accuracy
- [X] Try converting a model in TensorFlow and Pytorch to both ONNX and NNEF formats


## The execution

The first thing that I decided to attempt was the conversion of a model in Tensorflow into the ONNX formats. I decided to create a very simple model, that works on the MNIST dataset, so as to just understand the process, and not worry much about the Model itself. 
Now, the process to convert TensorFlow models to ONNX is explained pretty well in the ONNX Models [4] github site, and I believe me explaining won't make much sense, as you can jus read it from the Source itself. Similarly, for the NNEF frameworks, the documentation is very good, just refer to the NNEF Model Zoo [5] for clarity, as that'll explain it much better than my explanation xD.

But for my explanation,for ONNX Conversion, first create a TensorFlow model,and this[6] will help a lottt AND THEN, save the model.
Now, Convert a TensorFlow saved model with the command:
'python -m tf2onnx.convert --saved-model path/to/savedmodel --output dst/path/model.onnx --opset 13'
That's IT!!
For verification, you'll need to look at the ONNX github itself.

Now, for NNEF conversion, trust me, just read the documentation.

## References

[1] [https://github.com/JdeRobot/RoboticsAcademy](https://github.com/JdeRobot/RoboticsAcademy)\\
[2] [https://onnxruntime.ai/](https://onnxruntime.ai/)\\
[3] [https://www.khronos.org/nnef](https://www.khronos.org/nnef)\\
[4] [https://github.com/onnx/models](https://github.com/onnx/models)\\
[5] [https://github.com/KhronosGroup/NNEF-Tools/tree/master/models#nnef-model-zoo](https://github.com/KhronosGroup/NNEF-Tools/tree/master/models#nnef-model-zoo)\\
[6] [https://www.tensorflow.org/tutorials](https://www.tensorflow.org/tutorials)\\ 