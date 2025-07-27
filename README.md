erl_gp_sdf_msgs
=================

A ROS package that defines messages, services, and actions for [erl_gp_sdf](https://github.com/ExistentialRobotics/erl_gp_sdf).

# Getting Started

```shell
cd <your_workspace>/src
git clone https://github.com/ExistentialRobotics/erl_cmake_tools.git
git clone https://github.com/ExistentialRobotics/erl_gp_sdf_msgs.git
cd <your_workspace>
# for ROS1
catkin build erl_gp_sdf_msgs
# for ROS2
colcon build --packages-up-to erl_gp_sdf_msgs --cmake-args -DCMAKE_BUILD_TYPE=Release
```
