---
title: "Coding Period: Weeks 6"
excerpt: "Using Seaborn to get prettier plots"
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

Week 5 went pretty nicely, and then the only thing left was to work on using seaborn to get prettier plots, And I thought it'll be pretty easy, right?
BOY WAS I WRONG.


## Objectives

- [X] Check the codebase as well 
- [X] Use seaborn to get prettier plots
- [X] Updating the graph in real time


## The execution

The main idea that I thought, to implement Seaborn was to add these 2 lines:-
"import seaborn as sns" and 
"sns.set()", in the Evaluator.py in the benchmarking folder of the Human detection exercise and add the same in Exercise.py of the exercise. The exercise workings was explained to me shortly by my mentors, and some of it that I understood was from the REadme.md that is acailable in the ROboticsAcadmey github page [1]. As we can see, the understanding of the codebase is also here, and will be used even in the further weeks. Hence, you can never say that you can like understad the codebase completely, and I guess i will continue to add that in the Objectives section from now.
Now, overall, the code dodn't work in the normal way (i.e. through using the docker containers), as I wasn't able to create a Docker image, and hence, we decided to try it in the way where the docker container is not utilized, again suggested by my mentors. Trust me, if my mentors wouldn't have helped me with this, i would've been complete toast by now. Initially i was copying the path wrong, and then we realised that we were working in the wrong image, as that Image dodn't have the updated dockerfile contents (the image needs to download seaborn for it to work)
However, what I suggested was to try the code in my mentor's image, as for him it was working perfectly fine, and it worked for him. So, basically we tried a LOT of things, and we got the updated code working in 2 ways, one in the updated docker image, in my Mentor's device, and One in my laptop, with the exercise-not-being-connected-to-docker method. again helped by mentors here.

## References

[1] [https://github.com/JdeRobot/RoboticsAcademy](https://github.com/JdeRobot/RoboticsAcademy)\\
[2] [https://onnxruntime.ai/](https://onnxruntime.ai/)\\
[3] [https://www.khronos.org/nnef](https://www.khronos.org/nnef)\\
[4] [https://github.com/onnx/models](https://github.com/onnx/models)\\
[5] [https://github.com/KhronosGroup/NNEF-Tools/tree/master/models#nnef-model-zoo](https://github.com/KhronosGroup/NNEF-Tools/tree/master/models#nnef-model-zoo)\\
[6] [https://www.tensorflow.org/tutorials](https://www.tensorflow.org/tutorials)\\ 
[7] [https://github.com/tensorflow/models/tree/master/research/object_detection/models](https://github.com/tensorflow/models/tree/master/research/object_detection/models)\\
[1] [https://github.com/JdeRobot/RoboticsAcademy/blob/master/docs/InstructionsForDevelopers.md](https://github.com/JdeRobot/RoboticsAcademy/blob/master/docs/InstructionsForDevelopers.md)\\