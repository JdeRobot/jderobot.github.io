---
permalink: /projects/deep_learning/
title: "DeepLearning Suite"

sidebar:
  nav: "docs"

classes: wide
#toc: true
#toc_label: "TOC Projects"
#toc_icon: "cog"
---


<i class="fab fa-fw fa-github"></i> [**Detection Suite GitHub**](https://github.com/JdeRobot/DetectionSuite)
{: .notice--info}


DetectionSuite is a C++ on-development tool to test and train different **DeepLearning architectures for object detection** on images. It accepts several known international datasets like PASCALVOC and allows the comparison of several DeepLearning architectures over exactly the same test data. It computes several objective statistics and measures their performance. Currently it support YOLO architectures on Darknet framework.

{% include video id="gDP9nWCL0Vg" provider="youtube" %}


This is a tool for DeepLearning applications. Its development has its own public repository

- It accepts several image databases
- It allows fast annotation of object detection databases
- It shows statistics of neural network performance over images from several detection databases
- It may run networks from several DeepLearning middlware (YOLO...)



## DeepLearning Projects

- [Vinay Sharma (GSoC-2018)](https://jderobot.org/Club-VinaySharma) DeepLearning, DetectionSuite tool
- [Alexandre Rodriguez](https://jderobot.org/Arodriguez-tfm) (master): DeepLearning.
- [David Pascual](https://jderobot.org/Dpascual-tfm), (master): Convolutional Pose Machines.
- [Nuria Oyaga](https://jderobot.org/Noyaga-tfm), (master): Predicting images, learning time sequences.
- [Vanessa Fernández](https://jderobot.org/Vmartinezf-tfm) (master): Visual Control with DeepLearning.

[Pretrained network models](http://jderobot.org/store/deeplearning-networks/).
{: .notice--info}

## Challenges

Adding support for segmentation, more datasets and more DL frameworks.

The goal of this project is to expand the supported datasets (ImageNet, COCO...) and expand the neural frameworks (Keras, TensorFlow, Caffe...). In addition several detection architectures should be trained and compared with the new release of the tool.

The expected result is a new release of DetectionSuite tool extending the existing functionality for objection but also for two new deep learning problems: classification and segmentation including new statistics for each of them.