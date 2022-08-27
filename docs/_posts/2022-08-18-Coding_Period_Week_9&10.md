---
title: "Coding Period: Weeks 9 and 10"
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

Week 9 and Week 10 were mainly used to update the exercise frontend, along with the completion of the changing graphs feature.


## Objectives

- [X] Update the Frontend of the exercise 


## The execution

In the exercise [1], the first thing that was decided was to allow the user to select between multiple graphs, and as explained in the previous blog posts, I decided to stick with only 2. The next thing, was to allow the nice execution of the fucntions created by me, so that the user could see the graphs well. During these weeks, I found out the mistakes that I was making, and also my Mentor pointed them out to me as well.
While copying a websocket message, I copied the function that was calling the benchmark function twice, and didn't notice that. Hence, Benchmarking was being done twice, and it was taking twice as long for the graphs to load. 
The next error from my side was of not understanding the difference between the '=' and the '==' operator, while comparing 2 variables, so yes, I'm pretty dumb. Now, after fixing these errors, the functions were working pretty well, as in, were actually doing their job of executing properly, as intended. Now, the next thing that we decided to move on was to make the graph choosing div not available to the user until the benchmarking process was complete, so as to avoid a function being called when another function is already running. Here, I decided to use a while loop to disable the div, until the output header shows the message of benchamrking thread is closed. However, only the outer div did this, and the inner div was static for the entire work. This is where i am stuck regarding this one.
The next thing was to make the benchmarking thread close with a graph, so as to not make the user feel that the Exercise is stuck, and that was simple to do, as I only had to add a gui.dislpay function for this. 
The next, and probably final idea that we had in mind was to fix the calling of the output_headers, so as to print the correct thing when a graph is called, and also to
remove the previous message, when a function is running.

## References

[1] [https://github.com/JdeRobot/RoboticsAcademy](https://github.com/JdeRobot/RoboticsAcademy)\\

