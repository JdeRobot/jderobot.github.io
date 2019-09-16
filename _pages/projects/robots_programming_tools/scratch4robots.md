---
permalink: /projects/robotics_programming_tools/scratch4robots/
title: "Scratch4Robots"

sidebar:
  nav: "docs"

layout: archive

classes: wide
---

<i class="fab fa-fw fa-github"></i> [**Scratch4Robots GitHub**](https://github.com/JdeRobot/Scratch4Robots)
{: .notice--info}


## Introduction

This tool allows to program complex robots like TurtleBot or drones with the visual language Scratch. Regular blocks from Scratch can be used in applications with Scratch2JdeRobot. In addition several blocks for some robots have been also created and can be included in the applications.



{% include video id="gT-qt0Opwb4" provider="youtube" %}


### Blocks included in Scratch

| Name                  | Type            | Description                                                  |
| --------------------- | --------------- | ------------------------------------------------------------ |
| Wait () secs          | Control Block   | Pauses the script for the amount of time.                    |
| Forever               | Control Block   | A loop that will never end.                                  |
| if () then            | Control Block   | Checks the condition so that if the condition is true, the blocks inside it will activate. |
| if () Then, Else      | Control Block   | Checks the condition so that if the condition is true, the blocks inside the first C will activate and if the condition is false, the blocks inside the second C will activate. |
| Repeat ()             | Control Block   | A loop that repeats the specified amount of times.           |
| say ()                | Looks blocks    | Print what you enter as parameter.                           |
| Set () to ()          | Variable blocks | Sets the specified variable to the amount.                   |
| Insert () at () of () | List blocks     | Insert item in the selected position of indicated list.      |
| Item () of ()         | List blocks     | Returns the item stored in the indicated position.           |
| Add () to ()          | List blocks     | Insert item in the list.                                     |
| Delete () of ()       | List blocks     | Remove the item stored in the indicated position.            |


### Blocks for drones



| Name            | Type       | Inputs                                                       | Outputs             | Description                                                 |
| --------------- | ---------- | ------------------------------------------------------------ | ------------------- | ----------------------------------------------------------- |
| Pose3D          | Perceptive |                                                              | XYZ Position        | Get the value of the robot 3D position.                     |
| Color detection | Perceptive | Color                                                        | SIZEimg, Ximg, Yimg | Colored object in image.                                    |
| Stop robot      | Motion     |                                                              |                     | Reset all velocity values.                                  |
| Drone Take Off  | Motion     |                                                              |                     | Makes the drone take off.                                   |
| Drone Land      | Motion     |                                                              |                     | Makes the drone land.                                       |
| Drone Move      | Motion     | direction: (forward, back, up, down, left, right), speed: {velocity (integer)} |                     | Gives the drone a speed in the indicated direction.         |
| Drone Turn      | Motion     | direction: (left, right), speed: {velocity (integer)}        |                     | Gives the drone a turning speed in the indicated direction. |


### Blocks for TurtleBot


| Name                   | Type       | Inputs                                                    | Outputs                                       | Description                                               |
| ---------------------- | ---------- | --------------------------------------------------------- | --------------------------------------------- | --------------------------------------------------------- |
| Pose3D                 | Perceptive |                                                           | XYZ Position                                  | Get the value of the robot 3D position.                   |
| Color detection        | Perceptive | Color                                                     | SIZEimg, Ximg, Yimg                           | Colored object in image.                                  |
| Frontal Distance       | Perceptive |                                                           | The average measure of the frontal laser data | Get the average value for the values of the frontal laser |
| Robot Move             | Motion     | direction: (forward, back, left, right); speed: (integer) |                                               | Gives a speed in the indicated direction                  |
| Robot Turn             | Motion     | direction: (left, right); speed: (integer)                |                                               | Gives a turning speed in the indicated direction          |
| Drone Move to Position | Motion     | direction: (forward, back, left, right); meter: (integer) |                                               | Move robot the indicated meters in one direction          |



## Prerequisites

### Scratch 2.0

Download the scratch file [from here](https://scratch.mit.edu/scratchr2/static/sa/Scratch-456.0.2.air) and then double click to install it.


```bash
wget -O adobe-air.sh http://drive.noobslab.com/data/apps/AdobeAir/adobe-air.sh
chmod +x adobe-air.sh; sudo ./adobe-air.sh
```

### ROS

[Follow the ROS tutorial installation](http://wiki.ros.org/kinetic/Installation/Ubuntu).

### Python requirements

```bash
git clone https://github.com/JdeRobot/Scratch4Robots
cd Scratch4Robots
pip install -r requirements.txt
```


### Gazebo and worlds

Follow the [Gazebo tutorial installation](http://gazebosim.org/tutorials?tut=install_ubuntu).

With this line we get some prepared worlds based on ROS ready to use:

```bash
sudo apt-get install ros-${ROS_DISTRO}-kobuki-gazebo
```

## Installing

Check out the full installation video.

{% include video id="5JYuD8N0RBs" provider="youtube" %}


### Install out ROS package

```bash
sudo apt-get install ros-kinetic-scratch4robots
```

### Install Scartch4Robots extension to use in Scratch

In scratch keep pressing shift key while you click on "File" > "Import experimental HTTP extension" and add our extension. The extension will be stored in the "extension" directory of your package.

```bash
Note: This step is necessary each time you initialize Scratch
```

### Download the tool from git
 

```bash
git clone https://github.com/JdeRobot/Scratch4Robots.git
```

Now your package is ready to use.

## How to Use


1. Make a scratch project and save it.

2. Make the translation from Scratch to Python. Generate the code:
  ```bash
  rosrun scratch4robots scratch2python /path/to/your/scratchproject.sb2
  ```
  This command will generate the python script on your current work directory.


3. Launch the simulated world. For example:
  ```bash
  roslaunch kobuki_gazebo kobuki_empty_world.launch --screen
  ```

4. Execute the generated code. The generated code need a configuration file .yml as parameter, you will find some usefull configuration files in our git repository.
  ```bash
  ./myscratchfile.py /path/to/robot_ros.yml
  ```

5. Running an example. You have all you need for running the examples in the examples folder.



## How is this tool built?

### Translation from Scratch to Python

To perform the block translation we use the `Scratch2python.py` script that parse our blocks replacing them with their corresponding code in Python. This script uses kurt library to load the scratch project.

### How to add a new Scratch block to the extension

- Add block code to `scratch2robot.s2e`.

  ```bash
  ["", "move robot %m.robotDirections meters %n", "robot/move/meters", "forward", 1],
  ["r", "size of object", "camera/size"],
  ["r", "x position of object", "camera/x_pos"],
  ["r", "y position of object", "camera/y_pos"],
  ```

- Add block code to `scratch2python.py`.

  ```bash
  ['move robot {} meters {}', 'robot.move_meters("%s", %s)'],
  ['size of object', 'robot.get_size_object()'],
  ['x position of object', 'robot.get_x_position()'],
  ['y position of object', 'robot.get_y_position()'],
  ```

- Add block code to `robot.py` or `drone.py`.

  ```python
  def move_meters(self, direction, meters=None)
      //code  
  ```

  ```python
  def get_size_object(self):
      //code
      return size
  ```


  ```python
   def get_x_postion(self):
       //code
       return x_position
  ```

  ```python
   def get_y_position(self):
       //code
       return y_position
  ```


- Add block code to kurt extension in `commands_src_extras.py`.

```bash
[' ', 'move robot %m.robotDirections meters %n', 'Scratch2JdeRobot/robot/move/meters', 'forward', 1],
['r', 'size of object', 'Scratch2JdeRobot/camera/size'],
['r', 'x position of object', 'Scratch2JdeRobot/camera/x_pos'],
['r', 'y position of object', 'Scratch2JdeRobot/camera/y_pos'],
```


Note: You can find more information about how to create a extension in [ExtensionDoc](https://en.scratch-wiki.info/w/images/ExtensionsDoc.HTTP-9-11.pdf).

