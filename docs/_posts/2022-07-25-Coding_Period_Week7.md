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

gallery:
  - url: /assets/images/graphs_part1.png
    image_path: /assets/images/graphs_part1.png
    alt: "graph_image"
    title: "Image 1 title caption"

author: Bhavesh Misra
pinned: false


---



## Overview

Week 7 happened. Did not get kicked out of the Program. Very happy. Now have to work harder, so as to get everything done by the end of my GSoC duration. So basically I was able to pull through with the inclusion of Seaborn in the Exercise, and Now the aim was to understand the codebase (It will never be completley understood xD), and work on the next Objectives.


## Objectives

- [X] Check the codebase as well 
- [] Add more graphs in the Benchmarking section
- [] Update the Frontend of the exercise (like allowing the user to choose between different graphs) 


## The execution

The first thing that went through my mind, was to try and first do the HTML part of the code, i.e. adding a division and a list of all the possible options of graphs available. I decided to refer to [1] for this work. It was then decidied to have 3 graphs in total, they being mean Average Precision, 11-point Interpolation and Average Precision. After this, i explored Evaluator.py ,and found out that we can use 2 graphs, that are available to us, through changing the parameters passsed in the functions. Now, I decided to try both of these, and Got something like this.
<figure>
  <img src="/assets/images/graphs_part1.png" alt="graph_image">
  <figcaption>graph_image</figcaption>
</figure>

Now, the part that was left was to compile everything and get everything working, like getting the HTML, Javascript and the Python code ready, which I'm doing, and will be completed till week 8 (hopefully)

P.S. Tonikawa pretty wholesome stuff xD.

## References

[1] [https://cocodataset.org/#detection-eval](https://cocodataset.org/#detection-eval)
[2] [https://github.com/JdeRobot/RoboticsAcademy](https://github.com/JdeRobot/RoboticsAcademy)\\
[3] [https://onnxruntime.ai/](https://onnxruntime.ai/)\\
