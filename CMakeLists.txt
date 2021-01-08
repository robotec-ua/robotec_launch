cmake_minimum_required(VERSION 3.0.2)
project(robotec_launch)

## Find catkin macros and libraries
find_package(catkin REQUIRED COMPONENTS
  robotec_msgs
  geometry_msgs
  roscpp
  rospy
  std_msgs
)

## Specify additional locations of header files
include_directories(
  ${catkin_INCLUDE_DIRS}
)


###################################
## catkin specific configuration ##
###################################
catkin_package(
    
)