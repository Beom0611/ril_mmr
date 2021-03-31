# Robot Intelligence Lab_Mobile Manipulator (RIL_MM)
 
## Overview
This mobile manipulator(UR5 with Robotiq Gripper85 and Husky) tutorial will show you how to operate a mobile manipulator using Gazebo, RViz, MoveIt



### Before start this tutorial, please check your ROS version, this package for ROS Melodic version



## Guide

- For RIL_MM
[UR5+Robotiq Gripper85+Husky Model]  
```
$ cd ~/catkin_ws/src && git clone https://github.com/ros-industrial/universal_robot.git
$ cd ~/catkin_ws/src && git clone https://github.com/StanleyInnovation/robotiq_85_gripper.git
$ cd ~/catkin_ws/src && git clone https://github.com/husky/husky.git
$ cd ~/catkin_ws/src && git clone https://github.com/Beom0611/ril_mm.git
$ cd ~/catkin_ws && catkin_make
$ rosdep update
$ rosdep install --from-paths src --ignore-src -r -y
```


## Sample codes for beginners 
- Spawning RIL_MM in Gazebo and Rviz 
```  
$ roslaunch ril_mm_gazebo ril_mm_empty_world.launch
```
- Moving RIL_MMR to the goal point  
``` 
$ cd ~/catkin_ws/src/ril_mm_python   
$ chmod +x husky_point.py
$ rosrun ril_mm_python husky_point.py 
```
- Contorlloing the mobile manipuatlor's arm and gripper   
```
$ cd ~/catkin_ws/src/ril_mm_python
$ chmod +x joint_test1.py
$ rosrun ril_mm_python joint_test1.py 
```

**More Info**   
- **Sangbeom Park, [github]:https://github.com/Beom0611**  



## Description    

<img width="500" height="300" src="https://user-images.githubusercontent.com/78074831/109133146-08b8df80-7798-11eb-98a7-53325b398b83.png"  alt="Screenshot" title="Screenshot">
