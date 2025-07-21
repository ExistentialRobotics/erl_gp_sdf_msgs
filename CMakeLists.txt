cmake_minimum_required(VERSION 3.16)

project(erl_gp_sdf_msgs #
        LANGUAGES CXX C #
        VERSION 0.1.0 #
        DESCRIPTION "erl_gp_sdf_msgs is a ROS message package for SDF estimation.")
message(STATUS "Configuring ${PROJECT_NAME} ${PROJECT_VERSION}")

if (NOT COMMAND erl_project_setup)
    find_package(erl_cmake_tools REQUIRED)
endif ()
erl_project_setup()

erl_setup_ros(
    CATKIN_COMPONENTS std_msgs geometry_msgs message_generation #
    CATKIN_DEPENDS std_msgs geometry_msgs message_runtime #
    SRV_FILES SdfQuery.srv SaveMap.srv #
    MSG_DEPENDENCIES std_msgs geometry_msgs #
    ROS2_COMPONENTS std_msgs geometry_msgs)
erl_install()
erl_mark_project_found()
