# turtlesim_multi_waypoint
To move the turtle through multiple waypoints 
# To run the code:

1. To simulate turtlesim_multi_waypoint, the first step is to create a New ROS workspace
```Shell
  mkdir -p ~/catkin_ws/src
  cd  ~/catkin_ws/src
  catkin_make 
  source devel/setup.bash
   ```
2.After creating the workspace clone the repository
 ```Shell
 cd  ~/catkin_ws/src
 https://github.com/aleenalentin/Turtlesim_Multiple_Waypoint_control.git
 cd ..
 catkin_make
 ```
3.  Launch the nodes.
```Shell
 roslaunch turtle_control waypoint_follow.launch 
```
# Demo 

Click on the following image to see the demo video

[![Introduction Video](https://img.youtube.com/vi/j3yOLoU72Eg/0.jpg)](https://youtu.be/j3yOLoU72Eg)
