## Description
This git is addition application git for Open Manipulator.  
Original Reference Code is   
https://github.com/ROBOTIS-GIT/open_manipulator_simulations.git  

## environment setting 

*First you must set open manipulator   
```bash
sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-gazebo* ros-kinetic-moveit* ros-kinetic-dynamixel-sdk ros-kinetic-dynamixel-workbench-toolbox ros-kinetic-industrial-core  
```
*Sencond,  download modifed git and change. 
```bash
$git clone https://github.com/AuTURBO/open_manipulator_simulations.git  
$git clone https://github.com/hyunoklee/open_manipulator.git  
$git clone https://github.com/hyunoklee/dynamixel-workbench.git  
$git clone https://github.com/hyunoklee/dynamixel-workbench-msgs.git  
$git clone https://github.com/ROBOTIS-GIT/DynamixelSDK.git
$git clone https://github.com/ROBOTIS-GIT/open_manipulator_msgs.git
$git clone https://github.com/ROBOTIS-GIT/robotis_manipulator.git
```

*Third,  download and install packages about darknet ros and jsk. 
```bash
$git clone https://github.com/hyunoklee/darknet_ros.git
you unzip darknet.zip file at darknet directory.   
$git clone https://github.com/AuTURBO/turtlebot3_slam_3d
$git clone https://github.com/jsk-ros-pkg/jsk_common.git
$catkin_ws && catkin_make
$sudo apt-get install ros-kinetic-jsk-recognition
$sudo apt-get install ros-kinetic-libsiftfast
$sudo apt-get install ros-kinetic-laser-assembler
$sudo apt-get install ros-kinetic-octomap-server
$sudo apt-get install ros-kinetic-nodelet
$sudo apt-get install ros-kinetic-depth-image-proc
$sudo apt-get install ros-kinetic-jsk-topic-tools
$sudo apt-get install ros-kinetic-rtabmap-ros
```

## gazebo model information
  
I use warehouse model like below at beach world.   
https://3dwarehouse.sketchup.com/model/35757c0d1ded27425c459aad36b6b0c/beach  
https://3dwarehouse.sketchup.com/model/0de002ca-6220-44d7-8b87-54c396f8a511/Drink-19  
https://3dwarehouse.sketchup.com/model/cfb70c44-e8ea-46f2-8ec7-f564a775d342/BARRA-POINT  

## jjapit project 

<img src="/picture/1.png" width="70%" height="70%">    
Click image to link to YouTube video.    
[![Video Label](http://img.youtube.com/vi/J4-7gAYSDGI/0.jpg)](https://youtu.be/J4-7gAYSDGI?t=0s)     

* run  
```bash
$roscore
$roslaunch open_manipulator_gazebo open_manipulator_gazebo_jjapit.launch
$roslaunch open_manipulator_controller open_manipulator_controller.launch use_platform:=false
!!!!! please push play button gazebo window.  
if you want to pick apple, write below command.   
$roslaunch open_manipulator_example jjap_it.launch target_object:=apple
if you want to pick orange, write below command.   
$roslaunch open_manipulator_example jjap_it.launch target_object:=orange

```

## beach project  

<img src="/picture/2.png" width="70%" height="70%">  

* run  
```bash
$roscore  
$roslaunch open_manipulator_gazebo open_manipulator_gazebo_beach.launch  
$roslaunch open_manipulator_moveit open_manipulator_demo.launch use_gazebo:=true  
!!!!! please push play button gazebo window.  
```



