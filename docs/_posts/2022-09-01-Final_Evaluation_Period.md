---
title: "Coding Period: Final_Evaluation_Period"
excerpt: "Updating the exercise frontend"
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

The Final Evaluation Period was used to finish all the remaining tasks left in the Frontend part of the Exercise, along with testing the changes in the Docker container, instead of the conventional way of the non-docker Web template, and pusing the final changes to the RoboticsAcademy [1] Repository, by creating a pull request.


## Objectives

- [X] Update the Frontend of the exercise 
- [X] Test the exercise in the Docker Container
- [X] Complete the blog 

## The execution

In the exercise [1], the first thing that was decided was to allow the user to select between multiple graphs, and as explained in the previous blog posts, I decided to stick with only 2. The next thing, was to allow the nice execution of the fucntions created by me, so that the user could see the graphs well. After mentioning the meistakes that I made in the last blog, the thing that I wanted to do most, was to test these changes in the DOcker container, since I felt that the exercise was working fine in the non-docker Web template.
Now, me and my mentors had a meet, where they showed me hoe to move your changes in the docker container, and I'll explain those in this blog.
First, clone the latest repository, and move all your changes that you made in the non-DOcker Web template, in the latest Repository, like the changes in the python, html, javascript and the css files, without messing up the original structure of the repository (i.e., not deleting anything by mistake that was already there).
After this, run the Exercise using the Docker Run method, as shown in the Human_Detection [2] exercise in the terminal. Next, open a new ternimal, access the dockerfile by first checking the container_ID using the docker ps -a command, then executing the Containder, usng the docker exec "Container name" bash command. 
This process is just to see if the COntainer that you are running is the right one. Next, exit the bash script, and copy the contents using the docker cp command, like for example, "docker cp RoboticsAcademy_latest c4978c3ebc9e:/" by moving in the right directory that contains the Name of the repository that you want to move to the Docker container.
Next, open the terminal where the exercise is already running, and open the localhost link. You should be able to see your changes, being executed in the Docker Container. Keep in mind that the paths may differ for the non-docker Web-template, so make sure to change them.
Now, the task left for me is to create a review blog, where I review all the changes done by me, in the past 10 weeks

## References

[1] [https://github.com/JdeRobot/RoboticsAcademy](https://github.com/JdeRobot/RoboticsAcademy)\\
[2] [https://jderobot.github.io/RoboticsAcademy/exercises/ComputerVision/human_detection](https://jderobot.github.io/RoboticsAcademy/exercises/ComputerVision/human_detection)\\
