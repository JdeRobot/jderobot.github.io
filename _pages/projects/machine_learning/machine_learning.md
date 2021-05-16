---
permalink: /projects/machine_learning/
title: "Machine Learning in Robotics"

sidebar:
  nav: "docs"

classes: wide


feature_row:
  - image_path: /assets/images/projects/deep_learning/detection_suite.png
    alt: "Detection Metrics"
    title: "Detection Metrics"
    excerpt: "Set of tools to evaluate object detection neural networks models over the common object detection datasets."
    url: "https://jderobot.github.io/DetectionMetrics/"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/neural_behavior/autonomous.jpeg
    alt: "Behavior Metrics"
    title: "Behavior Metrics"
    excerpt: "Different types of neural networks that allow learning behavior "
    url: "https://jderobot.github.io/BehaviorMetrics"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/deep_learning/neural_fpga.png
    alt: "Neural FPGA"
    title: "Neural FPGA"
    excerpt: "Custom hardware able to do inference over generic neural networks using only open source tools."
    url: "/projects/deep_learning/neural_fpga/"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/deep_learning/object_detector.png
    alt: "Object Detector"
    title: "Object Detector"
    excerpt: "Easily window which simultaneously shows on real-time the image captured from a webcam or video ..."
    url: "/projects/deep_learning/object_detector/"
    btn_class: "btn--primary"
    btn_label: "Go!"
---




{% include feature_row %}





## MachineLearning Projects

- [**Reinforcement Learning Studio GitHub**](https://github.com/JdeRobot/RL-Studio)
- [Francisco Pérez](https://roboticslaburjc.github.io/2017-tfm-francisco-perez/) (master): DeepLearning in autonomous vision based navigation of real robots.
- [Nacho Arranz](https://roboticslaburjc.github.io/2019-tfm-ignacio-arranz/) (master): Deep Reinforcement Learning for autonomous car.
- [David Pascual](https://jderobot.org/Dpascual-tfm), (master): Convolutional Pose Machines.
- [Nuria Oyaga](https://jderobot.org/Noyaga-tfm), (master): Predicting images, learning time sequences.
- [Vanessa Fernández](https://jderobot.org/Vmartinezf-tfm) (master): Deep Learning for Visual Control.
- [Alexandre Rodriguez](https://jderobot.org/Arodriguez-tfm) (master): DeepLearning.
- [Vinay Sharma (GSoC-2018)](https://jderobot.org/Club-VinaySharma) DeepLearning, DetectionSuite tool

[Pretrained network models](http://wiki.jderobot.org/store/deeplearning-networks/).
{: .notice--info}

## Challenges

Adding support for segmentation, more datasets and more DL frameworks.

The goal of this project is to expand the supported datasets (ImageNet, COCO...) and expand the neural frameworks (Keras, TensorFlow, Caffe...). In addition several detection architectures should be trained and compared with the new release of the tool.

The expected result is a new release of DetectionStudio tool extending the existing functionality for objection but also for two new deep learning problems: classification and segmentation including new statistics for each of them.