---
permalink: /projects/robot_programming_tools/
title: "Robots Programming Tools"

sidebar:
  nav: "docs"

toc: true
toc_label: "TOC Projects"
toc_icon: "cog"


visual_circuit:
  - url: /assets/images/projects/robot_programming_tools/color_tuner.png
    image_path: /assets/images/projects/robot_programming_tools/fpga-circuit.png
    alt: "Visual Cirtuit 1"
  - url: /assets/images/projects/robot_programming_tools/icestudio.png
    image_path: /assets/images/projects/robot_programming_tools/icestudio.png
    alt: "Visual Cirtuit 2"
  

feature_row:
  - image_path: /assets/images/projects/robot_programming_tools/color_tuner.png
    alt: "Scratch4Robots"
    title: "Scratch4Robots"
    excerpt: ""
    url: "https://github.com/JdeRobot/Scratch4Robots"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/robot_programming_tools/color_tuner.png
    alt: "Color Tuner"
    title: "Color Tuner"
    excerpt: ""
    url: "https://github.com/JdeRobot/ColorTuner"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/robot_programming_tools/color_tuner.png
    alt: "3DViz"
    title: "3DViz"
    excerpt: ""
    url: "https://github.com/JdeRobot/3DViz"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/robot_programming_tools/color_tuner.png
    alt: "CamViz"
    title: "CamViz"
    excerpt: ""
    url: "https://github.com/JdeRobot/CamViz"
    btn_class: "btn--primary"
    btn_label: "Go!" 
  
  - image_path: /assets/images/projects/robot_programming_tools/color_tuner.png
    alt: "CarViz"
    title: "CarViz"
    excerpt: ""
    url: "https://github.com/JdeRobot/CarViz"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/robot_programming_tools/color_tuner.png
    alt: "DroneViz"
    title: "DroneViz"
    excerpt: ""
    url: "https://github.com/JdeRobot/DroneViz"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/robot_programming_tools/color_tuner.png
    alt: "PyOnBrowser"
    title: "PyOnBrowser"
    excerpt: ""
    url: "https://github.com/JdeRobot/PyOnBrowser"
    btn_class: "btn--primary"
    btn_label: "Go!"

  - image_path: /assets/images/projects/robot_programming_tools/color_tuner.png
    alt: "WebSim 2D"
    title: "WebSim 2D"
    excerpt: ""
    url: "https://github.com/JdeRobot/WebSim2D"
    btn_class: "btn--primary"
    btn_label: "Go!"


---

## Visual States

<i class="fab fa-fw fa-github"></i> [**VisualStates GitHub**](https://github.com/JdeRobot/VisualStates)
{: .notice--info}


[VisualStates](https://jderobot.github.io/VisualStates/) is a tool for programming **robot behaviors using automata**. It combines a graphical language to specify the states and the transitions with a text language (Python or C++). It generates a ROS node which implements the automata and shows a GUI at runtime with the active state every time, for debugging. 

<figure class="half">
    <a href=""><iframe src="https://www.youtube.com/embed/v5EMqtIyXlQ"></iframe></a>
    <a href=""><iframe src="https://www.youtube.com/embed/vUxjZ0CCmrM"></iframe></a>
    <figcaption>Visual States demo.</figcaption>
</figure>


### Visual States Projects

- [Pushkal Katara](https://jderobot.org/Club-PushkalKatara).


### Challenges

Adding full compatibility with ROS.

The current state of VisualStates only supports subscription and publish for topics. We aim to integrate all the communication features of the ROS and also basic packages that would be useful for behavior development. In the scope of this project the following improvements are targeted for a new release of VisualStates tool:

1. The integration of ROS services, the behaviors will be able to call ROS services.
2. The integration of ROS actionlib, the behaviors will be able to call actionlib services.
3. The generating and reading smach behaviors in VisualStates and modify and generate new behaviors.

**Library of parameterized automata**

Every automaton created using VisualStates can be seen as a state itself and then be integrated in a larger automata. Therefore, the user would be able to add previously created behaviors as states. When importing those behaviors, the user would have two options; copying the behavior on the new behavior or keeping reference to the imported automata such that if it is changed, those changes are going to be reflected on the new behavior too. The idea of this project is to built and support an automata library. There will be a library of predefined behaviors (automata) for coping with usual tasks, so the user can just integrate them as new states on a new automata, without writing any code. In addition, each automaton may accept parameters to fine tune its behavior. For example, for moving forward a drone, we'll have a state 'moveForward', so the user only have to import that state indicating as a parameter the speed he wants.

{% include video id="7yHDELR7sj4" provider="youtube" %}









## PyOnArduino: Compiling Python to Arduino language

<i class="fab fa-fw fa-github"></i> [**VisualStates GitHub**](https://github.com/JdeRobot/PyOnArduino)
{: .notice--info}


JdeRobot-Kids is an academic framework for teaching robotics to children in a practical way. It is based on Python, the kids have to program typical robot behaviors like follow-line using Python. JdeRobot-Kids is now mostly centered in the mbot robot, from makeblock, both the real robot and the simulated one in Gazebo. Mbot is an Arduino based robot. Currently the student application runs at a regular computer, which is connected to the onboard Arduino. Arduino and PC interact using the Firmata protocol. This approach requires a continuous connection between the robot and the off-board computer. Arduino is limited on computer power so it is not enough to run a Python interpreter. The goal of this project is to "compile" the Python application to Arduino microprocessor. This way the kid program can be fully downloaded on the Mbot robot and run completely autonomous. Another possibility is to translate Python application to C/C++, as gcc/g++ already compiles it to Arduino microprocessor. Some ideas to explore are: [LLVM](https://llvm.org) compiler infrastructure, [cython](https://cython.org)...



<figure class="half">
    <a href=""><iframe src="https://www.youtube.com/embed/k-xIU_cmcac"></iframe></a>
    <a href=""><iframe src="https://www.youtube.com/embed/_k17V5pxrd8"></iframe></a>
    <figcaption>PyOnArduino Projects.</figcaption>
</figure>


### PyOnArduino Projects

- [Sergio Paniego](https://jderobot.org/Club-spaniego).















## Visual Circuit Tool

<i class="fab fa-fw fa-github"></i> [**VisualStates GitHub**](https://github.com/JdeRobot/VisualCircuit)
{: .notice--info}


VisualCircuit is a tool for programming robot behaviors using a digital electronics language and abstractions. In reconfigurable circuits (FPGAs) a hardware description language is used to visually specify the circuit configuration and its behavior. For instance, the open source [IceStudio](https://github.com/FPGAwars/icestudio) tool uses such visual language to configure FPGAs. The idea of this project is to explore the use of the same visual language to program reactive robot behaviors. There are blocks (existing circuits) and wires to connect their inputs and outputs. 

Instead of synthesizing the visual program into a FPGA implementation the goal is to synthesize it into a Python program. Each block is translated into a thread that runs a transforming function at fast iterations. Each iteration reads the block inputs, does some specific processing to compute the right values and writes them on its outputs. Each wire is translated into a shared variable where the blocks can write or read. The expected result is a new tool to program reactive robot behaviors using a visual language based on blocks and wires.


{% include gallery id="visual_circuit" caption="Visual Circuit examples." %}



### Visual Circuits Projects

- [Sergio Lorenzo](https://jderobot.org/Slorenzo-tfg).















## FPGA Robots




## More Tools


{% include feature_row %}


