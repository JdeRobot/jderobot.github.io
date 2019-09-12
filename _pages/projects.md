---
layout: collection
permalink: /projects/

classes: wide

sidebar:
  nav: "docs"

#header:
#  overlay_color: "#5e616c"
#  overlay_image: /assets/images/cover/header.png
#  actions:
    #- label: "<i class='fas fa-download'></i> Install now"
    #  url: "/installation/"
#excerpt: 
#  Toolkit for developing Robotics and Computer Vision applications


projects:
  - image_path: /assets/images/projects/visual_states.png
    alt: "Robot Programming Tools"
    title: "Robot Programming Tools"
    excerpt: "Several development areas: robot programming tools, learning robotics, drones, SLAM algorithms, DeepLearning. All of them are open for collaboration."
    url: "/projects/robot_programming_tools/"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/robotics-academy-action.jpg
    alt: "Robotics Academy"
    title: "Robotics Academy"
    excerpt: "JdeRobot-Academy is an open source collection of exercises to learn robotics in a practical way. Programmed in Python, the Gazebo simulator and the ROS environment are used."
    url: "https://jderobot.github.io/RoboticsAcademy/"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/detection_suite.png
    alt: "Deep Learning"
    title: "Deep Learning"
    excerpt: "[DeepLearning Suite](https://github.com/JdeRobot/DetectionSuite) is a set of tool that simplify the evaluation of most common object detection datasets with several object detection neural networks."
    url: "/projects/deep_learning/"
    btn_class: "btn--primary"
    btn_label: "Go!" 
  
  - image_path: /assets/images/projects/fpga.jpg
    alt: "FPGAs in robotics"
    title: "FPGAs in robotics"
    excerpt: "[Neural FPGA project](https://github.com/JdeRobot/neuralFPGA) goal is to produce custom hardware able to do inference over generic neural networks. In order to test our hardware designs we rely on hardware simulations and FPGAs."
    url: "/projects/fpgas_in_robotics/"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/visual_slam.png
    alt: "Visual Slam"
    title: "Visual Slam"
    excerpt: "[VisualSLAM](https://github.com/JdeRobot/SDslam) uses computer vision to locate a 3D camera with 6 degrees of freedom inside a unknown environment and, at the same time, create a map of this environment."
    url: "/projects/visual_slam/"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/drones.png
    alt: "Drones"
    title: "Drones"
    excerpt: "The new Hardware Abstraction Layer (HAL) for working in robotic applications for Unmanned Aerial Vehicles (UAVs) in JdeRobot is based on using ROS/Gazebo, PX4 and MavROS."
    url: "/projects/drones/"
    btn_class: "btn--primary"
    btn_label: "Go!"   

---

Our (international) community mainly works on five development areas:

{% include feature_row_advanced %}