---
permalink: /projects/robots_programming_tools/visual_circuit_tool/
title: "Visual Circuit Tool"

sidebar:
  nav: "docs"

layout: archive

classes: wide



visual_circuit:
  - url: /assets/images/projects/robot_programming_tools/color_tuner.png
    image_path: /assets/images/projects/robot_programming_tools/fpga-circuit.png
    alt: "Visual Cirtuit 1"
  - url: /assets/images/projects/robot_programming_tools/icestudio.png
    image_path: /assets/images/projects/robot_programming_tools/icestudio.png
    alt: "Visual Cirtuit 2"
  
---



<i class="fab fa-fw fa-github"></i> [**VisualStates GitHub**](https://github.com/JdeRobot/VisualCircuit)
{: .notice--info}


VisualCircuit is a tool for programming robot behaviors using a digital electronics language and abstractions. In reconfigurable circuits (FPGAs) a hardware description language is used to visually specify the circuit configuration and its behavior. For instance, the open source [IceStudio](https://github.com/FPGAwars/icestudio) tool uses such visual language to configure FPGAs. The idea of this project is to explore the use of the same visual language to program reactive robot behaviors. There are blocks (existing circuits) and wires to connect their inputs and outputs. 

Instead of synthesizing the visual program into a FPGA implementation the goal is to synthesize it into a Python program. Each block is translated into a thread that runs a transforming function at fast iterations. Each iteration reads the block inputs, does some specific processing to compute the right values and writes them on its outputs. Each wire is translated into a shared variable where the blocks can write or read. The expected result is a new tool to program reactive robot behaviors using a visual language based on blocks and wires.


{% include gallery id="visual_circuit" caption="Visual Circuit examples." %}



### Visual Circuits Projects

- [Sergio Lorenzo](https://jderobot.org/Slorenzo-tfg).





