# MSFT-project-IBVS-through-Aruco
Author: Yanyin Yao, Kunyang Liang

Catkin_ws file structure of this workspace:

|--catkin_ws

|----src

|------doosan-robot

|------onrobot

|------manipulator_description

|------m0609_moveit_config

|------realsense

|----------realsense_ros

|----------realsense_ros_gazebo

|------my_scene

|----------aruco_ros

|----------arm_control

# Objective:
The aim of this VIBOT MSFT course project is to implement or simulate an eye-in-hand image-based visual servo control in Gazebo using a Doosan M0609 robotic arm manipulator with a camera mounted on its end effector. The visual features will be provided from 4-points in an Aruco tag.

# Preparation before simulation
## realsense package installation
According to the system environment, install realsense SDK and realsense_ros.

![屏幕截图 2024-01-08 235240](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/4a668f3f-2cdd-4719-bf68-fdbc0d2ab959)

## Add Aruco marker in gazebo environment
```bash
sudo cp tag_36.zip /usr/share/gazebo-11/models
```

# Gazebo + Moveit + doosan robotic arm + gripper simulation
In this part, we create the robot description using XACRO files and then loaded in a Gazebo simulation. The robot description is composed of a robot arm Doosan m0609, a robot gripper OnRobot RG2 and a color camera. 
![屏幕截图 2024-01-07 195401](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/89122b5b-170f-4b4a-9f6a-cce484beb552)

![屏幕截图 2024-01-08 200132](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/2038900f-b044-491d-88d9-3229edc7703e)

## Moveit
we use the third-party software MoveIt to define robot arm motion trajectories.

![屏幕截图 2024-01-07 194514](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/39de1a45-7ed7-4593-9a97-04d1eee2a956)

![屏幕截图 2024-01-07 195159](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/9ce9ff1f-b7de-4d71-aedd-0d903ed7d51c)

```bash

roslaunch m0609_moveit_config dsr_moveit_gazebo.launch

```
![GIF 2024-1-8 15-11-28](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/97932e61-bc4c-4355-a237-45ad8048dccf)

# Testing the aruco_ros package using Realsense
![屏幕截图 2024-01-08 174857](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/37e95521-f9a5-4e11-bc63-9fef0ec92cbf)

![屏幕截图 2024-01-08 150957](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/a36cb63d-1d01-44e1-9285-a2c74f85f07a)

# IBVS-through-Aruco
