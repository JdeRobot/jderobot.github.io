---
permalink: /projects/drones/drones/
title: "Drones"

sidebar:
  nav: "docs"

layout: archive

classes: wide
---


## Tools for drones in JdeRobot

The drone can be teleoperated from a smartphone. The images of the onboard cameras are shown in the smartphone


{% include video id="fEuhzmRH-Fs" provider="youtube" %}


## Using ROS/MavROS with PX4 SITL and 3DR Solo simulation in Gazebo

Installation instructions [here](https://github.com/JdeRobot/assets/tree/master/drones). Please note that this is a first approach, if you encounter any issues report them in the [JdeRobot's github repository](https://github.com/jderobot/jderobot).

### Stage 1: Launching the 3DR Solo simulation. Testing basic functionalities: Arm motors, takeoff, hover and land


- Goal: After installing PX4 SITL for ROS/Gazebo and MavROS 0.25.1, some testing using the 3DR Solo simulation, MavLINK 2.0 and the MavROS tools mavsafety (for arming motors) and mavcmd (for taking off and landing)

- **Status**: Almost finished

- **Achieved**:

  1. Link between PX4 SITL and MavROS node obtained:
    - Use `roslaunch mavros px4.launch fcu_url:="udp://:14540@127.0.0.1:14557"`
    - Link working checked by echoing the `/mavros/diagnostics` topic
  2. Arm 3DR Solo motors with `rosrun mavros mavsafety arm`.
  3. Take off in `PX4 AUTO.RTL` flight mode
    - Using global latitude,longitude coordinates (LOCAL_NED frame) available at /mavros/fake_gps/geo_origin parameters
    - Use `rosrun mavros mavcmd takeoff pitch yaw lat lon alt`. Important: `rosrun mavros mavcmd takeoffcur pitch yaw alt` doesn't work (GPS fix is compulsory)

- **Pending**:

  - Keep drone hovering by solving the No Datalink issue, that triggers failsafe and RTH + Auto Landing
  - Tried changing PX4 flight mode from AUTO.RTL to OFFBOARD. PX4 present flight mode is published in the /mavros/state topic.
  - To change it, first publish any `/mavros/setpoint` with `rostopic pub -r 20 ...` and then use `rosrun mavros mavsys mode -c OFFBOARD`.
  - Unfortunately, once in OFFBOARD mode, RTH still triggers due to *No Datalink*.
  - Possible solution: Try changing NAV_RCL_ACT parameter to 0.


- **Demonstration**
  {% include video id="wiVFPPJuaow" provider="youtube" %}


## Stage 2: Use OFFBOARD PX4 Mode. Keep drone hovering. Land safely.

- **Goal**: Find the right sequence of mavROS commands to enter OFFBOARD Mode, take off, keep drone hovering for a while and land safely. In OFFBOARD PX4 mode, the drone obeys a position, velocity or attitude setpoint provided over MAVLink by an "external" computer. The main characteristics of OFFBOARD mode can be found [here](https://docs.px4.io/en/flight_modes/offboard.html).

- **Status**: Finished

- **Achieved**: The right sequence of commands to enter OFFBOARD mode is as follows:

  1. The drone must receive a stream of target setpoints at a rate greater than 2 Hz before entering OFFBOARD mode. Run first `rostopic pub -r 20 /mavros/setpoint_position/local...` and include a PoseStamped ROS message with the local height (for example: `x=0 y=0 z=2`).
  2. The drone must be armed before engaging OFFBOARD. Run `rosrun mavros mavsafety arm`.
  3. Engage OFFBOARD mode by `rosrun mavros mavsys mode -c OFFBOARD`. The drone will then take off (see the *Note* below)
  4. Send other setpoints, if any, using the right ROS topics (position, velocity, attitude)
  5. Land using `rosrun mavros mavcmd land 0 0 0 0` . The drone exits OFFBOARD mode and enters AUTO.LAND mode

  *Note*: This is not the only way of doing it. The taking off sequence, can be done by first taking off and then enter OFFBOARD mode, but there is a risk of triggering RTH due to the No Datalink issue.

- **Demonstration**
  {% include video id="FPX13Ks5xmA" provider="youtube" %}


### STAGE 3: Using relative cmd_vel velocity commands in OFFBOARD mode.

- **Goal**: Test cmd_vel relative velocity commands by changing the PX4 FRAME from LOCAL_NED to BODY_FRAME. Available mavlink frames are listed [here](https://github.com/mavlink/mavros/blob/master/mavros_msgs/srv/SetMavFrame.srv).

- **Status**: Ongoing.

- **Achieved**: Relative velocity commands are feasible in MavROS!

    1. Key: changing the PX4 FRAME to BODY_FRAME using `rosservice call /mavros/setpoint_velocity/mav_frame "mav_frame: 8"`
    2. After that, take off in OFFBOARD mode using the procedures available below (in STAGE 2)
    3. The drone will read the velocity setpoints sent by publishing a cmd_vel "Twist" ROS message at the /mavros/setpoint_velocity/cmd_vel_unstamped/ topic as "relative" velocities (i.e. as given in its local reference frame)
  
  In the example below, a circular trajectory is proven just by using linear_vx=1 + angular_vz=1, with all other speed components = 0

- **Demonstration**
  {% include video id="FEZ81GShvB0" provider="youtube" %}
  


## Object Tracking

Several examples of visual control using JdeRobot:

### Tracking a moving object in the ground.

This tracking algorithm is able to maintain the position and orientation of the drone while the object moves along the ground. The control system is divided in two subsystems: control position only (x,y) and control orientation only (theta). The first one use control curves to command speed to the drone. The second one uses a control surface for the rotations of the drone. Both subsystems work together to track down the object.

{% include video id="UqEOn0mZ0Uc" provider="youtube" %}


### Object Tracking in 3D

In this tracking algorithm, the drone tracks down a red ball in a 3D space. The algorithm use three PID controllers to maintain the position of the drone.

{% include video id="pZJa6olGOlc" provider="youtube" %}

### Following a road

{% include video id="rIkTImMyoXw" provider="youtube" %}


## Precise Landing.

The drone takes off, searches the beacon (it is on an unknown location) and lands on it. It uses its onboard camera to detect the beacon and a visual control to smoothly land on it.

{% include video id="VOi3ao5O7xk" provider="youtube" %}

## Path Following.

So far only in simulation. The red line is the path to follow, the green one is the estimated position and the blue line is the real position given by the simulation environment.

{% include video id="PGzx-qOkmpg" provider="youtube" %}



## Programming contest

We have organized two editions of the Program-A-Robot contest. The participants have to program a drone (the cat) to pursue another autonomous drone (the mouse). Take a look to [Competitions](/activities/competitions/) section.