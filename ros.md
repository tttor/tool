# [ROS](http://ros.org/)
## ros cmd
* system
  * `catkin_create_pkg beginner_tutorials std_msgs rospy roscpp`
  * `catkin_make`
* controller
    * `rosrun controller_manager controller_manager list`
    * `rosservice call /controller_manager/list_controller_types`
* tf
  * `rosrun tf tf_echo /map /odom`
  * `rosrun tf view_frames`
  
## clean_catkin_ws
```
#!/bin/bash
# http://wiki.ros.org/catkin/Tutorials/using_a_workspace#Cleaning_up
# https://answers.ros.org/question/66366/how-to-catkin_make-clean-just-one-package/
rm -rf build devel install
```
