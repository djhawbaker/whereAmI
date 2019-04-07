# Where Am I
Robo Nano Degree: Where Am I robot localization project

Using the robot and world from previous projects this one adds robot localization with Adaptive Monte Carlo Localization (AMCL)

To run, setup two terminals
1. cd catkin_ws
2. catkin_make
3. source devel/setup.bash

Run in separate terminals 
1. roslaunch my_robot world.launch 
2. roslaunch my_robot amcl.launch

Then do one of the following
1. Set a 2D Nav Goal in RViz
2. Setup another terminal and run (This option requires the teleop package as well)
  - rosrun teleop_twist_keyboard teleop_twist_keyboard.py  

The Robot will find itself on the provided map by driving around and using AMCL with it's sensors to localize.
