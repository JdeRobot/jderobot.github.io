---
permalink: /projects/visual_slam/
title: "Visual SLAM"

sidebar:
  nav: "docs"

layout: archive

classes: wide
---

<i class="fab fa-fw fa-github"></i> [**Visual SLAM GitHub**](https://github.com/JdeRobot/SDslam)
{: .notice--info}

Simultaneous Localization and Mapping (SLAM) algorithms play a fundamental role for emerging technologies, such as autonomous cars or augmented reality, providing an accurate localization inside unknown environments. There are many approaches available with different characteristics in terms of accuracy, efficiency and robustness ([ORB-SLAM](http://webdiis.unizar.es/~raulmur/orbslam/), [DSO](https://vision.in.tum.de/research/vslam/dso), [SVO](http://rpg.ifi.uzh.ch/svo2.html), etc), but their results depend on the environment and resources available.


## Slam-TestBed tool

**Slam-TestBed** is a graphic tool to compare objectively different Visual SLAM approaches, evaluating them using several public benchmarks and statistical treatment, in order to compare them in terms of accuracy and efficiency. The main goal of this project is to increase the compatibility of this tool with new benchmarks and SLAM algorithms, so that it becomes an standard tool to evaluate future approaches.

The next video shows one of the SLAM algorithms (called ORB-SLAM) that will be evaluated with this tool:

{% include video id="ufvPS5wJAx0" provider="youtube" %}

## MapGenerator

Create realistic 3D maps from SLAM algorithms. SLAM algorithms provide accurate localization inside unknown environments, however, the maps obtained with these techniques are often sparse and meaningless, composed by thousands of 3D points without any relation between them.

![](/assets/images/projects/visual_slam/slam-fusion.png){: .align-center}


The goal of this project is to process the data obtained from SLAM approaches and create a **realistic 3D map**. The input data will consist of a dense 3D point cloud and a set of frames located in the map. The next video shows one of the SLAM algorithms (called DSO) whose output data will be used to create the 3D map. The expected result of this project is a tool for building realistic 3D maps from a 3D point cloud and frames.

<figure class="half">
    <a href="/assets/images/cover/projects.png"><iframe src="https://www.youtube.com/embed/xwSOOdqQ"></iframe></a>
    <a href="/assets/images/cover/activities.jpg"><iframe src="https://www.youtube.com/embed/Y5bIL-qN6uE"></iframe></a>
    <figcaption>Visual SLAM examples.</figcaption>
</figure>



### Visual SLAM Projects

- [Elías Barcia](https://jderobot.org/Elias-tfm) (master): Visual SLAM, slam-testbed.
- [Jianxiong Cai](https://jderobot.org/Club-jianxiong) (GSoC-2018) Creating realistic 3D map from online SLAM result.

