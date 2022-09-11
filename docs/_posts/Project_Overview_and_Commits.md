---
layout: post
title:  "Project Overview  and Commits"
date:   2022-09-10 02:30:50 +0530
categories: jekyll update
---

## What was done

I worked on building a Deep Learning Human Detection Exercise to identify the presence of humans and identification of the rectangular boundary around them. Apart from the live and video inference features, the exercise also includes model benchmarking and model visualization. The user is expected to upload a Deep Learning model which fits the required input and output specifications for inference. The input model is supposed to be in the ONNX format. <br/>
The project work also included compiling and testing an exercise guide for the user, which contains everything from fine tuning pre built object detection models in different frameworks(PyTorch and TensorFlow), to its subsequent conversion to the ONNX format. <br/> <br/>
Below is a very brief timeline of the work done. For more information and details, please refer to the specific week in the blog post. <br/>

| Week      | Work Done |
| ----------- | ----------- |
| **Community Bonding Period**      | Tried Working with the Exercise to get a good fell for the changes needed, along with setting up the Environment for the Deep learning exercise to run successfully.       |
| **Week 1**   | Understanding the ONNX and NNEF formats to represent Machine Learning Models, along with converting different models to these formats        |
| **Week 2 and 3**      | Researched different Models that are used for Object Detection, and deciding which one to be used for the Exercise        |
| **Week 4**      | Converting the said model (the SSDLite_MObilenet Model to the ONNX format, updating the blog with all the work done till now        |
| **Week 5**  | Implementing the Seaborn library in the Exercise, basically trying to get prettier plots for the user to understand.         |
| **Week 6**      | Working for the Midsem Evaluation, by documenting whatever done till now       |
| **Week 7 and 8**   | Understanding the Codebase to work better, as now the work was mainly frontend-related, along with adding different graphs in the picture, so as to give the user more understanding. Started working on creation of a list where the user can change Graphs manually         |
| **Week 9 and 10**   | Week 9 and Week 10 were mainly used to update the exercise frontend, along with the completion of the changing graphs feature. Compiling the results, and DOcumenting everything done till now for the End-Semester Evaluation       |

## Working Demo

<iframe width="700" height="480"
src="https://www.youtube.com/embed/vn4ahq8mElg">
</iframe> 
<br/>

## Merged PR's 

* [Allow users to choose between different metrics in benchmarking mode (Issue #1791)](https://github.com/JdeRobot/RoboticsAcademy/pull/1803)
* [Use seaborn to improve benchmarking plots readability #1763](https://github.com/JdeRobot/RoboticsAcademy/pull/1788)

## Extras

* [Added the SSD_Volumenet_lite v2 model for the HumanDetection Exercise](https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/tree/main/The%20SSDlite_mobilenetV2_model)
* [Converted a tensorflow model to .nnef format](https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/blob/main/tf_to_nnef.ipynb)
* [Converted a tensorflow model to .onnx format](https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/tree/main/some%20.ipymbs)
