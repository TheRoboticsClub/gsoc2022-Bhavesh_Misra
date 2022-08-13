---
title: "Coding Period: 8"
excerpt: "Extension of Week 7"
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

gallery:
  - url: https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/blob/main/docs/assets/images/graphs_part1.png
    image_path: https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/blob/main/docs/assets/images/graphs_part1.png
    alt: "graph_image"
    title: "Image 1 title caption"

  - url: https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/blob/main/docs/assets/images/graphs_part2.png
    image_path: https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/blob/main/docs/assets/images/graphs_part2.png
    alt: "graph_image_many"
    title: "Image 2 title caption"    
---

## Overview

Week 8 is just an extension of week 7, where the task of completing the objectives of week 7 was the only task. 


## Objectives

- [X] Check the codebase as well 
- [X] Add more graphs in the Benchmarking section
- [X] Update the Frontend of the exercise (like allowing the user to choose between different graphs) 


## The execution

The first thing that went through my mind, was to try and first do the HTML part of the code, i.e. adding a division and a list of all the possible options of graphs available. I decided to refer to [1] for this work. It was then decidied to have 3 graphs in total, they being mean Average Precision, 11-point Interpolation and Average Precision. After this, i explored Evaluator.py ,and found out that we can use 2 graphs, that are available to us, through changing the parameters passsed in the functions. Now, I decided to try both of these, and Got something like this.
<figure>
  <img src="https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/blob/main/docs/assets/images/graphs_part1.png" alt="graph_image">
  <figcaption>graph_image</figcaption>
</figure>
(From Week 7 itself, Week 8 is just an extension of the work for week 7)

Now, to add more Graphs in the benchmarking section, I first decided to go in the exercise.py and the Emulator.py section of the RoboticsAcademy exercise github, to see and understand what all graphs are available to the users. Here, i found out about EveryPointInterpolation, and the ElevenPointInterpolation methods to plot the graphs. I decided to add an entire section for the Average Precision, similar to the above mentioned methods.
Now, after adding my method, I ran the exercise and I realised that it took a LOT more time to get the graph for Average Precision, as compared to the other graphs. 
So, I decided to completely drop the idea, and decided to move forward with 2 graphs, instead of 3.
Now, the next step was to create a list in HTML, and then using javascript to get the value that the user chooses form the list using the Document.getElementByID Function, and use the Websocket to pass a message everytime the user selects an option from the list, and print a graph as per the User's preference.
However, All of this is happening, BUT only 1 time, when the user tries to change the option,the graphs don't change. I am not able to completely unserstand the reason for this.

<figure>
  <img src="https://github.com/TheRoboticsClub/gsoc2022-Bhavesh_Misra/blob/main/docs/assets/images/graphs_part2.png" alt="graph_image_many">
  <figcaption>graph_image</figcaption>
</figure>
 
P.S.1 Tonikawa pretty wholesome stuff xD.
P.S.2 Violet Evergarden OST REALLY GOOD!!

## References

[1] [https://cocodataset.org/#detection-eval](https://cocodataset.org/#detection-eval)
[2] [https://github.com/JdeRobot/RoboticsAcademy](https://github.com/JdeRobot/RoboticsAcademy)\\
[3] [https://onnxruntime.ai/](https://onnxruntime.ai/)\\
