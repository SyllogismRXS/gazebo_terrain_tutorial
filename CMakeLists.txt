cmake_minimum_required(VERSION 3.0.2)
project(gazebo_terrain_tutorial)

find_package(catkin REQUIRED COMPONENTS
  gazebo_ros
)

catkin_package(
  CATKIN_DEPENDS
  gazebo_ros
)

install(DIRECTORY launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

install(DIRECTORY models
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

install(DIRECTORY worlds
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
