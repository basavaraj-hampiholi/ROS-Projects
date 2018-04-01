Simulation of single robot in Stage simulator:

Please follow the below steps:
1. Create a catkin workspace
2. Download/clone the git repository catkin source directory
3. Build the files using catkin workspace
4. Open the terminal and run
      source catkin_ws/devel/setup.bash
5. Run 'roscore' from terminal
6. Open new terminal and run,
      roslaunch myrobot turtlebot_in_stage.launch
7. Input value of X and Y values(coordinates of map). Make sure that 
   there are no obstacles. If you provide a point where the obstacle is present,
   the robot will start 'rotate recovery' and will not lead to anywhere.
   
8. In case of no obstacle, Robot reaches the goal and notifies you about the same.
   
