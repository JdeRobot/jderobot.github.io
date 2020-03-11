---
layout: splash
permalink: /
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/cover/header.png
  #actions:
  #  - label: "<i class='fas fa-github'></i> GitHub"
  #    url: "https://github.com/JdeRobot"
  #  - label: "<i class='fas fa-github'></i> Twitter"
excerpt: 
  Open toolkit for developing Robotics applications
feature_row:
  - image_path: /assets/images/cover/projects.png
    alt: "Projects"
    title: "Projects"
    excerpt: "Several development areas: robot programming tools, DeepLearning, FPGAs, Education, drones, SLAM algorithms. Open for collaboration."
    url: "/projects/"
    btn_class: "btn--primary"
    btn_label: "Learn more"

  - image_path: /assets/images/cover/activities.jpg
    alt: "Activities"
    title: "Activities"
    excerpt: "Some of the activities of the organization where students from different areas come together to put together a common project."
    url: "/activities/"
    btn_class: "btn--primary"
    btn_label: "Learn more"   

  - image_path: /assets/images/cover/community.jpg
    alt: "Community"
    title: "Community"
    excerpt: "The JdeRobot organization is open to contributions at development, documentation, testing, integration and research."
    url: "/community/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
youTube_id: ID7qaEcIu4k

---


<figure class="third" style="text-align: center">
    <a href="https://github.com/JdeRobot" target="_blank"><img src="/assets/images/cover/github_social_button.png" style="width:200px;"></a>
    <a href="https://twitter.com/jderobot" target="_blank"><img src="/assets/images/cover/twitter_social_button.png" style="width:200px;"></a>
    <a href="https://www.youtube.com/channel/UCgmUgpircYAv_QhLQziHJOQ/videos" target="_blank"><img src="/assets/images/cover/youtube_social_button.png" style="width:200px;"></a>
</figure>

{% include feature_row %}

Robotics applications are typically distributed, made up of a collection of concurrent asynchronous components which communicate using some middleware (ROS messages, ICE, DDS...). Building robotics applications is a complex task. Integrating existing nodes or libraries, which provide already solved functionality, and using several tools may increase the software robustness and shorten the development time. JdeRobot toolkit provides several tools, libraries and reusable nodes for Robotics and Computer Vision.

| Main Features |
| :--- |
| ROS friendly (full compatible with ROS-Kinetic) |
| C++, Python, JavaScript |
| Open Source |
| Easy installation from debian, PIP and npm packages |


Our (international) community mainly works on six fields inside Robotics and Computer Vision:

<style type="text/css">
.mytable{text-align: center}
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;border-color:black;}
.tg .tg-lboi{border-color:inherit;text-align:left;vertical-align:middle;}
.tg .tg-kmbl{font-weight:bold;background-color:#c0c0c0;color:#000000;border-color:inherit;text-align:center;vertical-align:middle}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top;}
</style>

<div class="mytable">
<table class="tg">
  <tr>
    <th class="tg-kmbl"><a href="http://jderobot.org/Projects#Robot_Programming_Tools">Development Areas</a></th>
    <th class="tg-kmbl"><a href="http://jderobot.org/Projects#Robot_Programming_Tools">Products</a></th>
  </tr>
  <tr>
    <td class="tg-lboi" rowspan="2"><a href="https://jderobot.github.io/projects/robotics_education">Robotics education and games</a></td>
    <td class="tg-0pky"><a href="https://jderobot.github.io/RoboticsAcademy/">Robotics-Academy</a> for engineering students</td>
  </tr>
  <tr>
    <td class="tg-0pky">Kibotics online platform for children learning robotics</td>
  </tr>
  <tr>
    <td class="tg-lboi" rowspan="2"><a href="https://jderobot.github.io/projects/deep_learning">DeepLearning</a> in robotics</td>
    <td class="tg-0pky"><a href="https://jderobot.github.io/DetectionSuite">DetectionSuite </a>tool for evaluation of visual detection networks</td>
  </tr>
  <tr>
    <td class="tg-0pky"><a href="https://github.com/JdeRobot/ObjectDetector">ObjectDetector </a>see deep learning networks in action</td>
  </tr>
  <tr>
    <td class="tg-lboi" rowspan="2">FPGAs in robotics</td>
    <td class="tg-0pky"><a href="https://github.com/JdeRobot/neuralFPGA">neuralFPGA </a>running deeplearning networks on FPGAs</td>
  </tr>
  <tr>
    <td class="tg-0pky"><a href="https://github.com/JdeRobot/FPGA-robotics">FPGA-robotics </a>designing robot intelligence with IceStudio blocks</td>
  </tr>
  <tr>
    <td class="tg-lboi" rowspan="1">Drones</td>
    <td class="tg-0pky"><a href="https://wiki.jderobot.org/Drones">Drones</a> infrastructure and applications</td>
  </tr>
  <tr>
    <td class="tg-lboi" rowspan="2"><a href="https://jderobot.github.io/projects/robots_programming_tools">Robot Programming Tools</a></td>
    <td class="tg-lboi"><a href="https://jderobot.github.io/VisualStates">VisualStates </a>tool for robot programming with automata</td>
  </tr>
  <tr>
    <td class="tg-0pky"><a href="https://github.com/JdeRobot/WebSim2D">WebSim2D </a>robot simulator with web technologies</td>
  </tr>
  <tr>
    <td class="tg-lboi" rowspan="2"><a href="https://jderobot.github.io/projects/visual_slam/visual_slam">SLAM</a>, visual localization</td>
    <td class="tg-0pky"><a href="https://github.com/JdeRobot/SDslam">SDslam </a>visual SLAM algorithm</td>
  </tr>
  <tr>
    <td class="tg-0pky"><a href="https://github.com/JdeRobot/slam-TestBed">slam-testbed </a>tool for evaluation of SLAM algorithms<br></td>
  </tr>
  </table>

</div>

We are registered as **non-profit organization** in Spain Ref.#615800.

## News

* **JdeRobot has been accepted as a mentoring organization for Google Summer of Code 2020**, several students will be funded by Google to work in open projects of our organizaton. Check the [proposed ideas list](https://jderobot.github.io/activities/gsoc/2020) and our candidate selection process.
* The last stable release, JdeRobot-5.7.0, has been released as debian package (2020/02/14): full compatible with ROS Melodic.
<!-- * All our web pages are finally being migrated to GitHub Pages: nice, under version control and convenient. -->
<!-- * JdeRobot was accepted as a mentoring organization for Google Summer of Code 2019, several students will be funded by Google to work in open projects of our organizaton. Check the [proposed ideas list](https://jderobot.github.io/activities/gsoc/2019) and our candidate selection process. --> 
<!--  * The last stable release, [JdeRobot/base 5.6.7](https://github.com/JdeRobot/base/wiki/JdeRobot-5.6.7) has been released (2019/03/12): full compatible with ROS Kinetic. -->
<!-- * 3rd edition of [Program-A-Robot Challenge](https://jderobot.github.io/activities/competitions/2018) was celebrated inside the [International Conference on Intelligent Robots and Systems (IROS 2018)](https://www.iros2018.org/competitions) (2018/10/03). Watch the [summary video](https://www.youtube.com/watch?v=VFBL6zuXqgo): a drone (cat) searches and pursues a moving target (mouse). -->


<div align="center">
  <a class="twitter-timeline" data-lang="en" data-width="800" data-height="700" href="https://twitter.com/JdeRobot?ref_src=twsrc%5Etfw">Tweets by JdeRobot</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
</div>


<figure class="half">
    <a href="/assets/images/cover/projects.png"><iframe src="https://www.youtube.com/embed/gDP9nWCL0Vg"></iframe></a>
    <a href="/assets/images/cover/activities.jpg"><iframe src="https://www.youtube.com/embed/1iYlJLJkESU"></iframe></a>
<!--    <figcaption>Last two videos from YouTube channel.</figcaption> -->
</figure>

## Roadmap

We are working on:

* Update of underlying infrastructure: jump to Ubuntu 18.04, ROS Melodic Morenia, Gazebo9 simulator, Python 3.5.
* Use of reconfigurable hardware (FPGAs) in robotics, with third party open tools like IceStudio
* [VisualStates tool](https://jderobot.github.io/VisualStates) for visual programming of the robot intelligence with Finite State Machines. It creates a C++ or a Python component from the visual description of the automata.
<!-- * Scratch4Robots tool for programming of TurtleBot and drones using Scratch visual language -->
* [RoboticsAcademy](https://jderobot.github.io/RoboticsAcademy): a framework to learn robotics and computer vision with drones, autonomous cars.... It is a collection of Python programmed exercises. Include a web service for this.
* (*done*) <del>All our web pages are finally being migrated to GitHub Pages: nice, under version control and convenient</del>
* (*done*) <del>Compatibility with ROS robotics middleware: interoperation between ROS nodes and JdeRobot components, use of ROS drivers, use of ROS bag files... JdeRobot (>= 5.6) is fully compatible with ROS Kinetic including its official debian packages</del>
* (*done*) <del>Update of underlying infrastructure: jump to Ubuntu 16.04, OpenCV-3, migration to Gazebo-7 simulator (revisit existing plugins and models), PCL-1.8, ICE-3.6</del>
* (*done*) <del>Use of Web technologies in robotics: ICE-JS, WebRTC, HTML5, electron, nodeJS... </del> Many webtools have been developed: viewers, teleoperators and drivers.


## License

* <img src="/assets/images/cover/GPLv3.png" style="width:200px;"> JdeRobot is open source. All its code is licensed under GPL v3.
* <img src="/assets/images/cover/CC_BY-SA_3.0.png" style="width:200px;"> All the documentation of JdeRobot project is licensed under Creative Commons by-sa 

## Sponsors

<figure class="third">
    <a href="https://summerofcode.withgoogle.com" target="_blank"><img src="/assets/images/cover/GSoC.png" style="width:400px;"></a>
    <a href="http://www.qualoom.es" target="_blank"><img src="/assets/images/cover/logo_qualoom.png" style="width:400px;"></a>
    <a href="https://urjc.es" target="_blank"><img src="/assets/images/cover/logoURJC.jpg" style="width:400px;"></a>
</figure>

<figure class="third">
    <a href="https://twitter.com/roboticslaburjc" target="_blank"><img src="/assets/images/cover/peloto3-sinletra.png" style="width:150px;"></a>
</figure>