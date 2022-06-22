# turtlesim_multi_waypoint
To move the turtle through multiple waypoints 
# To run the code:

1. Create a new ROS workspace
```Shell
 mkdir -p ~/catkin_ws/src
   ```
2. Clone the code 
 ```Shell
 cd  ~/catkin_ws/src
 https://github.com/aleenalentin/Turtlesim_Multiple_Waypoint_control.git
 ```
3. Return to workspace root
 ```Shell
 cd ../

   ```
4. Build the workspace 
```Shell
cd ~/catkin_ws/
catkin_make 

``` 
5.  Launch the nodes.
```Shell
roslaunch turtle_control waypoint_follow.launch 
```
# Demo 

Click on the following image to see the demo video

[![Introduction Video](https://img.youtube.com/vi/j3yOLoU72Eg/0.jpg)](https://youtu.be/j3yOLoU72Eg)
