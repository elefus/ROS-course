cmake_minimum_required(VERSION 2.8.3)
project(lab4)


find_package(catkin REQUIRED COMPONENTS
  roscpp
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES lab4
#  CATKIN_DEPENDS roscpp
#  DEPENDS system_lib
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)


add_executable(lab4 src/teleop.cpp)


target_link_libraries(lab4
  ${catkin_LIBRARIES}
)