---
title: "Community Bonding: Week 3"
excerpt: "Continuing - resolving issues and adding features in main tools"
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

I identified some errors while using the existing frameworks. This week, we will continue to fix the issues found and discussed during the meeting. I also verified the inference time for PilotNet model (PyTorch implementation), the difference between the CPU vs GPU execution is (0.0265  vs 0.0192) seconds (mean inference time) for simulation of 1 minute.

![ ]({{ site.url }}{{ site.baseurl }}/assets/images/sim_stat_metrics.png)

When we save stats of a simulation a window shows all metrics in details. We will also use this in later phases to evaluate and compare our optimized models. I describe our new objectives next.


## Objectives

- [ ] Solve the issue [Error while trying to save stats with DL-torch.yml config #368](https://github.com/JdeRobot/BehaviorMetrics/issues/368) and sumbit a PR
- [ ] Fix the issue [Not utilizing GPU when running simulation #369](https://github.com/JdeRobot/BehaviorMetrics/issues/369).
- [ ] Update PR [updated package versions for python3.10 #46](https://github.com/JdeRobot/DeepLearningStudio/pull/46) to remove additional packages and include installation instructions in REAMDE
- [ ] Update PR [Use new dataset #49](https://github.com/JdeRobot/DeepLearningStudio/pull/49) - Add feature to let user specify each dataset directory and normalize label values.
- [ ] Update PilotNet brain in BehaviorNet to unnormalize (expand) the predicted values
- [ ] Implement evaluation on the validation set in training scripts of models

## Issues and Pull requests.
*

## The execution



## References

[1] [https://github.com/JdeRobot/BehaviorMetrics](https://github.com/JdeRobot/BehaviorMetrics) \\
[2] [https://github.com/JdeRobot/DeepLearningStudio](https://github.com/JdeRobot/DeepLearningStudio)
