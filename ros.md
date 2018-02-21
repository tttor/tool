# [ROS](http://ros.org/)
## ros cmd
* system
  * `catkin_create_pkg beginner_tutorials std_msgs rospy roscpp`
  * `catkin_make`
  * `catkin_make --pkg <package A> <package B>` # warn: not robust, see [this](https://answers.ros.org/question/54178/how-to-build-just-one-package-using-catkin_make/)
  * `rostopic list | grep -o -P '^.*(?=/feedback)'` # list action servers from [this](https://answers.ros.org/question/222748/list-action-servers/)
* controller
    * `rosrun controller_manager controller_manager list`
    * `rosservice call /controller_manager/list_controller_types`
* tf
  * `rosrun tf tf_echo <source_frame> <target_frame>`
  * `rosrun tf tf_monitor <source_frame> <target_target>`
  * `rosrun tf view_frames` # generate a pdf
  
## clean_catkin_ws
```
#!/bin/bash
# http://wiki.ros.org/catkin/Tutorials/using_a_workspace#Cleaning_up
# https://answers.ros.org/question/66366/how-to-catkin_make-clean-just-one-package/
rm -rf build devel install
```
