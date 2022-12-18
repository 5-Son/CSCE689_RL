# CSCE689_RL

ROS package to control TurtleBot in Gazebo simulation using RL-PID control.

## 1. Environment
- Ubuntu 20.04, ROS Noetic
  
## 2. Package Documentation

**TurtleBot 3**  
https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/

## 3. Package Installation

- **TurtleBot3 on Gazebo**  
	1.Follow the tutorials from the ROBOTIS website.
	https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/

	1. Clone *turtlebot_rl_py* package into workspace  
		`cd ~/catkin_ws/src`  
		`git clone https://github.com/5-Son/CSCE689_RL.git`
    
	2. Build 'catkin' workspace directory  
		`cd ~/catkin_ws`  
		`catkin_make`
    
	3. Install python dependencies  
		`pip3 install numpy transforms3d`

## 4. Execute ROS Packages
- **Waypoint Navigation using RL PID control on Gazebo Sim**  
	Package: *turtlebot_rl_py*
	1. Start the TurtleBot3  Gazebo simulation
  		`export TURTLEBOT3_MODEL=burger`  
  		`roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch`
  
	2. Execute the python script  
		`rosrun turtlebot_rl_py waypoint_test.py`  
