cmake_minimum_required(VERSION 3.0.2)
project(sim_demo)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  xacro
  gazebo_ros
  joint_state_publisher
)

catkin_package(
  # 这里如果有库或消息可以填
)

# 如果你后面写了自己的 C++ 节点，就在这里添加：
# include_directories(${catkin_INCLUDE_DIRS})
# add_executable(my_node src/my_node.cpp)
# target_link_libraries(my_node ${catkin_LIBRARIES})

install(DIRECTORY meshes urdf worlds launch config
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

