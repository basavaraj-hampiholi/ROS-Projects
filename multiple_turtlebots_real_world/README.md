# Simulation of simultaneous navigation of 2 real robots under namespace

Please follow the below steps:

I. Connect the turtlebot to workstation

   https://www.youtube.com/watch?v=1KOrXSEDQ3k
   The connection is established between single Master(workstation) and two slaves(turtlebots) as per the above tutorial video
   
II. On Workstation:
1. Create a catkin workspace
2. Download/clone the git repository catkin source directory
3. Build the files using catkin workspace
4. Open the terminal and run source catkin_ws/devel/setup.bash
5. Run 'roscore' service
6. Launch Rviz to view navigation
7. Go to step III.1(On Turtlebot)
8. Run the 'scripts/patrol_organizer.py'. Robot will start rotate recovery and then move to the specified coordinates(in code)
   Check this independently on each robot. If both are working fine and then run 'scripts/patrol_organiser_both.py' and check
   whether both robots are moving simultaneously.


III. On Turtlebot:

1. Create a catkin workspace
2. Download/clone the git repository catkin source directory
3. Place robot_0 files in one turtlebot and robot_1 on the other turtlebot and perform the below steps.
3. Build the files using catkin workspace
4. Open the terminal and run source catkin_ws/devel/setup.bash
5. Open new terminal and run, roslaunch navigation_under_namespace robot_under_namespace.launch
6. goto step II.8(On Workstation)
7. Repeat the same for robot_1 
