cmake_minimum_required(VERSION 2.8.3)
project(racecar_gazebo)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages

find_package(catkin REQUIRED COMPONENTS
  gazebo_ros
  geometry_msgs
  roscpp
  cv_bridge
  image_transport
	message_generation
	message_runtime  
)


catkin_package(CATKIN_DEPENDS message_generation message_runtime roscpp)    


include_directories(
  include
  ${catkin_INCLUDE_DIRS}
  ${OpenCV_INCLUDE_DIRS}
)


