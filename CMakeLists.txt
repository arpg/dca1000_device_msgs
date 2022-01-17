cmake_minimum_required(VERSION 3.0.2)
project(dca1000_device_msgs)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
  std_srvs
  message_generation
)

 add_message_files(
  FILES
  MimoMsg.msg
  RadarCubeMsg.msg
 )

 generate_messages(
  DEPENDENCIES
  std_msgs
  std_srvs
)


catkin_package(
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

