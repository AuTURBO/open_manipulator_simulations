## Description
This git is addition application git for Open Manipulator.  
Original Reference Code is   
https://github.com/ROBOTIS-GIT/open_manipulator_simulations.git  

## environment setting 

*First you must set open manipulator   
http://emanual.robotis.com/docs/en/platform/openmanipulator/  

*Sencond,  download modifed git. 
```bash
git clone https://github.com/hyunoklee/open_manipulator.git  
git clone https://github.com/AuTURBO/open_manipulator_simulations.git  
```

## gazebo model setting
  
Move gazebo models in gazebo_model folder to ~/.gazebo/models.  
 
```bash
$cp -r ~/catkin_ws/src/open_manipulator_simulations/gazebo_model ~/.gazebo/models
```
I use warehouse model like below.   
https://3dwarehouse.sketchup.com/model/35757c0d1ded27425c459aad36b6b0c/beach  
https://3dwarehouse.sketchup.com/model/0de002ca-6220-44d7-8b87-54c396f8a511/Drink-19  
https://3dwarehouse.sketchup.com/model/cfb70c44-e8ea-46f2-8ec7-f564a775d342/BARRA-POINT  

## jjapit project 

<img src="/picture/1.png" width="70%" height="70%">  

* run  
```bash
$roscore  
$roslaunch open_manipulator_gazebo open_manipulator_gazebo_jjapit.launch  
$roslaunch open_manipulator_moveit open_manipulator_demo.launch use_gazebo:=true  
!!!!! please push play button gazebo window.  
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



