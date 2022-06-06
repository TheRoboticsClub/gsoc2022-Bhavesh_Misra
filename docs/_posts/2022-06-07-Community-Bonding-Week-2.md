---
title: "Community Bonding: Week 2"
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
- Behavior Metrics
- DL Studio

author: Nikhil Paliwal
pinned: false
---


## Preliminaries

Through the discussion, we identify potential issues which need to be worked on before the start of the coding period. We also took a diver dive into the working of Dockers to continuously support the Behavior Metric tool. While I explore the [Quick Start](https://jderobot.github.io/BehaviorMetrics/quick_start/) section, I identify interesting scripts `show_pilots.py` and other features to visualize the performance and save the stats of the deep learning model. Furthermore, the mentors introduced me to the development of [new dataset](https://github.com/JdeRobot/DeepLearningStudio/tree/main/Formula1-FollowLine) on DeepLearningStudio [2]. After I mention an improvement in the training script, we agreed to include a validation set. In the coming weeks, we would also like to benchmark the existing models on my local machine to set a baseline for optimized models.

## Objectives

- [X] Resolve dependency issue on DeepLearningStudio's virtual environment installation
- [X] Fix Dockerfiles to build the workflow in Behavior Metric
- [X] Explore the `show_pilots.py` script and report the relevance of it for the project
- [X] Update the `PilotNet` (PyTorch) model to use new dataset in DeepLearningStudio [2]
<!-- - [ ] Implement evaluation on the validation set in training scripts of models -->

## Issues and Pull requests.
* Created issue [Dependency conflict while installation #45](https://github.com/JdeRobot/DeepLearningStudio/issues/45) in DeepLearningStudio repo.
* Solved [issue #45](https://github.com/JdeRobot/DeepLearningStudio/issues/45) with PR [updated package versions for python3.10 #46](https://github.com/JdeRobot/DeepLearningStudio/pull/46) in DeepLearningStudio repo.
* Solved docker issues with PR [Fixes failing build of Docker images (with GPU support) in the workflow #365](https://github.com/JdeRobot/BehaviorMetrics/pull/365) in BehaviorMetric repo.
* I got errors while using `show_pilots.py` and created corresponding issue [KeyError while using show_plots.py script #366](https://github.com/JdeRobot/BehaviorMetrics/issues/366).
* Created another issue [Errors using 'scripts/analyse_brain.bash' #367](https://github.com/JdeRobot/BehaviorMetrics/issues/367).
* I encountered additional errors while using PilotNet (Pytorch) brain, for which I created additional issues - [Error while trying to save stats with DL-torch.yml config #368](https://github.com/JdeRobot/BehaviorMetrics/issues/368) and [Not utilizing GPU when running simulation #369](https://github.com/JdeRobot/BehaviorMetrics/issues/369).
* Create issue [Update PilotNet model to use new F1 dataset #48](https://github.com/JdeRobot/DeepLearningStudio/issues/48).
* Fixed the issue [Update PilotNet model to use new F1 dataset #48](https://github.com/JdeRobot/DeepLearningStudio/issues/48) by PR [Use new dataset #49](https://github.com/JdeRobot/DeepLearningStudio/pull/49). 

## The execution

My initial task includes upgrading Python version and related packages in the DeepLearningStudio repository and submitted PR [updated package versions for python3.10 #46](https://github.com/JdeRobot/DeepLearningStudio/pull/46). Next, I worked on the issues with docker images in BehaviorMetric repository, by locally buidling, resolving errors and creating containers and then submitted PR [Fixes failing build of Docker images (with GPU support) in the workflow #365](https://github.com/JdeRobot/BehaviorMetrics/pull/365). Building and fixing Dockers is especially time consuming (each build trial could takes hours). I encountered additional errors while using BehaviorMetrics for which I created corresponding issues and some solutions. The new dataset is relatively large (~ 11 GB), so extracting and managing will take time. I also updated corresponding scripts for PilotNet model in DeepLearningStudio to use new dataset.

## References

[1] [https://github.com/JdeRobot/BehaviorMetrics](https://github.com/JdeRobot/BehaviorMetrics) \\
[2] [https://github.com/JdeRobot/DeepLearningStudio](https://github.com/JdeRobot/DeepLearningStudio)