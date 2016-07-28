cmake_minimum_required(VERSION 2.8.3)
project(libp8_platform)

# You cloned with git clone --recursive, right?
add_subdirectory(lib/p8-platform)

find_package(catkin REQUIRED)

catkin_package(
  INCLUDE_DIRS lib/p8-platform/src
  LIBRARIES p8-platform
)
