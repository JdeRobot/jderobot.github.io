---
permalink: /projects/robotics_programming_tools/visual_states/
title: "Visual States"

sidebar:
  nav: "docs"

layout: archive

classes: wide
---


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





