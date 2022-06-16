cmake_minimum_required(VERSION 3.0.2)
project(turtle_control)

find_package(catkin REQUIRED COMPONENTS
  geometry_msgs
  message_generation
  roscpp
  rospy
  std_msgs
  turtlesim
)



## Generate messages in the 'msg' folder
add_message_files(
  FILES
  TurtleVel.msg
)

## Generate services in the 'srv' folder
add_service_files(
  FILES
  VelTranslate.srv
)



## Generate added messages and services with any dependencies listed here
generate_messages(
  DEPENDENCIES
  geometry_msgs
  turtlesim
)



catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES turtle_control
  CATKIN_DEPENDS geometry_msgs message_runtime roscpp rospy std_msgs turtlesim
#  DEPENDS system_lib
)


## Specify additional locations of header files
## Your package locations should be listed before other locations
include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)




catkin_install_python(PROGRAMS
 
  nodes/waypoint
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)




## Mark other files for installation (e.g. launch and bag files, etc.)
install(DIRECTORY launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
  FILES_MATCHING PATTERN "*.launch"
)

