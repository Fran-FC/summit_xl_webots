cmake_minimum_required(VERSION 2.8.3)
project(summit_xl_webots)


find_package(catkin REQUIRED COMPONENTS 
    roscpp
    std_srvs
    std_msgs
    tf
    joint_state_controller
    velocity_controllers
)


###################################
## catkin specific configuration ##
###################################
catkin_package(

)


#############
## Install ##
#############


install(
  DIRECTORY launch worlds rviz
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)


