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
