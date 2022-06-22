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



![gif](https://user-images.githubusercontent.com/20817830/174976499-ccb751a5-70d0-417c-af4f-c149c0283808.gif)


