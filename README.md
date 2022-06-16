<start>
roscore
source ./devel/setup.bash

-----------------------------------------------------------------------
<keyboard>
export TURTLEBOT3_MODEL=burger
roslaunch morobot_teleop morobot_teleop_key.launch

<joy>
rosrun joy joy_node
python ~/catkin_ws/src/PS4_Joystick_teleop_Mobile_Robots_ROS_Python/Joyteleop_turtlebot3.py

-----------------------------------------------------------------------

<hector Slam>
roslaunch morobot_bringup morobot_G2.launch
roslaunch morobot_slam morobot_slam_G2.launch
roslaunch morobot_slam morobot_slam_rviz.launch

<map save>
rosrun map_server map_saver -f map

<navigation>
roslaunch morobot_bringup morobot_G2.launch
roslaunch morobot_navigation morobot_navigation_G2.launch
roslaunch morobot_navigation morobot_navigation_rviz.launch


