---
permalink: /projects/deep_learning/object_detector/
title: "Object Detector"

sidebar:
  nav: "docs"

classes: wide
#toc: true
#toc_label: "TOC Projects"
#toc_icon: "cog"
---



<i class="fab fa-fw fa-github"></i> [**Object Detector GitHub**](https://github.com/JdeRobot/dl-objectdetector)
{: .notice--info}


`dl-objectdetector` is a JdeRobot node, composed of 3 entities: Camera, GUI and DetectionNetwork, which have been implemented on an asynchronous design with its own thread. As a result, we have an easily window which simultaneously shows on real-time the image captured from a webcam or video (via OpenCV) or remote proxy (through a ROS/ICE communicator, coming from the JdeRobot suite), and the same image with bounding boxes on it, surrounding the objects which the TF/Keras Neural Network has detected on it (yielding the detection score as well). Also, this continuous video detection flow can be easily stopped via a couple of buttons on the GUI, and turn the component to do on-demand detection.

This has been developed on a way which allows the Neural Network to be implemented as a Python class (DetectionNetwork()), which can be extracted from the component and used to load and use any kind of model, and even handle real-time and on-demand detection, via the thread (ThreadNetwork()). This can have really useful applications, some of which will be developed soon!