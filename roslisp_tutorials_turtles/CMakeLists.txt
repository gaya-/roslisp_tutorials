cmake_minimum_required(VERSION 2.8.3)
project(roslisp_tutorials_turtles)

find_package(catkin REQUIRED COMPONENTS
  roslisp
  turtlesim
  geometry_msgs
)


################################################
## Declare ROS messages, services and actions ##
################################################


###################################
## catkin specific configuration ##
###################################

catkin_package()


###########
## Build ##
###########

include_directories(
  ${catkin_INCLUDE_DIRS}
)

add_lisp_executable(circle turtles-system turtles-lisp-pkg:turtle-circle)


#############
## Install ##
#############


#############
## Testing ##
#############

