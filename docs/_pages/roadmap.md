---
permalink: /roadmap/

title: "Roadmap"

sidebar:
  nav: "docs"
---

# Optimization of Deep Learning models for autonomous driving


## Abstract

The main aim of the project is to improve the current model stack of deep learning
models, in terms of inference speed with minimum loss of precision, for autonomous driving applications. JdeRobot organization has created Behavior Metrics[1], a tool for comparing deep learning architectures for autonomous driving on different circuits with the support of Gazebo and Ros Noetic. The organization also provide another tool called DeepLearningStudio [2], which has datasets and model implementations for training deep learning models. We will use available tools and techniques such as TensorRT [3], Quantization [4], Pruning [5], and architectural changes [6,7,8] to optimize the correct model stack available in both PyTorch and Tensorflow.


### References

[1] [https://github.com/JdeRobot/BehaviorMetrics](https://github.com/JdeRobot/BehaviorMetrics) \\
[2] [https://github.com/JdeRobot/DeepLearningStudio](https://github.com/JdeRobot/DeepLearningStudio) \\
[3] [https://developer.nvidia.com/tensorrt](https://developer.nvidia.com/tensorrt) \\
[4] [https://www.tensorflow.org/api_docs/python/tf/quantization/quantize](https://www.tensorflow.org/api_docs/python/tf/quantization/quantize) \\
[5] [https://www.tensorflow.org/model_optimization/guide/pruning](https://www.tensorflow.org/model_optimization/guide/pruning) \\
[6] MobileNetV2: Inverted Residuals and Linear Bottlenecks.” 2018 [https://arxiv.org/abs/1801.04381](https://arxiv.org/abs/1801.04381) \\
[7] Deep Compression: Compressing Deep Neural Networks with Pruning, Trained Quantization and Huffman Coding [https://arxiv.org/abs/1510.00149](https://arxiv.org/abs/1510.00149) \\
[8] Knowledge Distillation [https://intellabs.github.io/distiller/knowledge_distillation.html](https://intellabs.github.io/distiller/knowledge_distillation.html)