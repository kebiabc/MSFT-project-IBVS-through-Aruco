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

![屏幕截图 2024-01-08 200132](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/853b68a1-f37f-4481-867c-72ed0b6d7b4b)
![image](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/e484f166-97ed-4e7d-882b-d5d8e13ef36a)
![屏幕截图 2024-01-08 174857](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/304acd06-4cc6-4221-854c-28b124c41a19)
![屏幕截图 2024-01-08 150957](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/f6af6c6c-6e21-4f40-8ec3-fc0bcc7d29a2)
![屏幕截图 2024-01-07 195401](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/a28ae5e8-49c0-405c-86fd-2d6d6072b262)
![屏幕截图 2024-01-07 195159](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/0c28253c-5c16-407d-a148-9089f9603583)
![屏幕截图 2024-01-07 194514](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/345a84a4-537e-4ae7-85a4-83f5d7d1ac42)
![GIF 2024-1-8 15-11-28](https://github.com/kebiabc/MSFT-project-IBVS-through-Aruco/assets/33951067/b212dc86-0fc7-4a10-bb93-06e729a40e3e)
