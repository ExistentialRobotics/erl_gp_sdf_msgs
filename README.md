erl_gp_sdf_msgs
=================

A ROS package for geometry messages to transmit data structures in erl_geometry.

# Install

```shell
cd <your_ros_ws>/src
git clone https://github.com/ExistentialRobotics/erl_cmake_tools.git
git clone https://github.com/ExistentialRobotics/erl_gp_sdf_msgs.git
cd <your_ros_ws>
# for ROS1
catkin build erl_gp_sdf_msgs
# for ROS2
colcon build \
    --event-handlers console_cohesion+ --cmake-args -DCMAKE_VERBOSE_MAKEFILE=ON \
    --cmake-clean-cache --packages-up-to erl_gp_sdf_msgs
```
