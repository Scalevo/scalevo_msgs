cmake_minimum_required(VERSION 2.8.3)
project(scalevo_msgs)
find_package(catkin REQUIRED COMPONENTS std_msgs sensor_msgs message_generation)

# add_message_files(
#  FILES
#)
add_service_files(
  FILES
  Starter.srv
)

generate_messages(DEPENDENCIES std_msgs sensor_msgs)

catkin_package(CATKIN_DEPENDS std_msgs sensor_msgs)
