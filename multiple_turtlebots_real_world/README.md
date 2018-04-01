# multiple robots in stage simulator
## Simulation of navigating three robots to the specific locations

Please follow the below steps:

1. Create a catkin workspace

2. Download/clone the git repository catkin source directory

3. Build the files using catkin workspace
 
4. Open the terminal and run
   source <catkin_ws>/devel/setup.bash

5. Run 'roscore' from terminal

6. Open new terminal and source again `setup.bash` and run,
   roslaunch multiple_robots_stage robots_in_stage.launch

7. Open new instance of terminal and run python patrol_organizer.py (situated in folder `multiple_robots_in_stage_sim/scripts`)

8. Robots will start move to the specified locations in the code