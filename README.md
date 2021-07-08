# SLAM-map-navigation
using SLAM map to launch the navigation 

## steps to run the navigation 
### 1.Launch Simulation World
this command will open the gazebo
```
$ export TURTLEBOT3_MODEL=waffle_pi
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch
```
### 2.Run Navigation Node

```
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml
```
### 3.Estimate Initial Pose
this step should be befor running the navigation
- click [2D Pose Estimate] in the RViz menu
- click in the robot location in the map and drag the green arrow toward the direction where the robot is facing.
- 
### 4.Set Navigation Goal
-now click on the [2D Nav goal] in RViz menu.
-click on the map to set the destination of the robot and drag the arrow toward the direction where the robot will be facing. 

![navigarionturtlebot3](https://user-images.githubusercontent.com/85634104/124968092-e3818b00-e02d-11eb-8c02-a4cee3a1ce0c.png)
