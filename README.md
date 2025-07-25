Autonomous Mecanum Wheeled Robot for Indoor Surveillance

This project showcases the development of an autonomous indoor surveillance robot equipped with Mecanum wheels for omnidirectional movement and powered by the Robot Operating System (ROS). The robot combines AI-based object detection, real-time motion planning, and environment simulation to navigate and monitor complex indoor environments autonomously.

🔧 Key Features

Omnidirectional Navigation using Mecanum wheels for precise movement in tight spaces

Real-Time Object Detection with YOLOv3 integrated into a 3D vision pipeline using an RGB-D camera

Sensor Fusion combining LiDAR, IMU, and depth data to enhance localization and obstacle avoidance

Custom Path Planning & Motion Control algorithms for stable and adaptive navigation

Simulation & Testing in Gazebo with real-time visualization using RViz

🛠️ Technologies Used

ROS1 Noetic (Robot Operating System)

Gazebo (robot simulation)

Python, C++

YOLOv3, OpenCV (for object detection)

Intel RealSense Camera (or equivalent RGB-D sensor)

RViz (real-time diagnostics and visualization)

🧠 Functional Highlights

Autonomous patrol and surveillance in indoor environments

Dynamic obstacle avoidance using camera and sensor data

Live visualization of robot state, sensor feeds, and planning output

Modular ROS node structure for navigation, perception, and control

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Getting Started
 To experience this project on your local machine, follow these steps: 
1. Install ROS Noetic by following the step-by-step tutorial provided here: [ROS Noetic Installation](https://wiki.ros.org/noetic/Installation/Ubuntu). 
2. Create a ROS workspace:
```
mkdir  catkin_ws/src 
cd catkin_ws 
catkin_make
```
3. Clone the world repository into your workspace:
```
cd ~/catkin_ws/src
git clone https://github.com/aswathisajeev97/Mecanum_four_wheeled_robot--Autonomous-driving.git
cd ~/catkin_ws && catkin_make
```
4. Launch the project using the launch command:
```
roslaunch car_description move_base.launch
```
## Usage 
Follow these steps to use the project: 
1. Launch mecanum robot model in RViz with joint state publisher GUI:
```
roslaunch car_description display.launch
```
2.  Launch mecanum robot in gazebo simulator with environment:
```
roslaunch car_description gazebo.launch
```
3. Launch mecanum robot in both gazebo and RViz:
```
 roslaunch car_description move_base.launch
```
