cmake_minimum_required(VERSION 3.8)
project(subt_cave_sim)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY models worlds
  DESTINATION share/${PROJECT_NAME}
)

ament_package()
