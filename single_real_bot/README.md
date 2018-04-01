# Moving a real turtlebot to a specified loaction

Please follow the below steps:

I. Connect the turtlebot to workstation

  https://www.youtube.com/watch?v=1KOrXSEDQ3k
  
II. On Turtlebot:   

1. Create a catkin workspace
2. Download/clone the git repository catkin source directory
3. Build the files using catkin workspace
4. Open the terminal and run
      source catkin_ws/devel/setup.bash
5. Run 'roscore' from terminal
6. Open new terminal and run,
      roslaunch single_real_bot minimal.launch
7. Open new terminal and run,
      roslaunch single_real_bot amcl_demo.launch map_file:=/home/turtlebot/catkin_ws/src/single_real_bot/my_map.yaml
   Provide the proper location of map file

III. On Workstation:

1. Create a catkin workspace
2. Download/clone the git repository catkin source directory
3. Build the files using catkin workspace
4. Open the terminal and run
        source catkin_ws/devel/setup.bash
5. Run the scripts/go_to_specific_point.py. It asks you to input X and Y values(coordinates of the maps).
   Try to input the coordinates where there is no obstacle.
   Robot will start rotate recovery in case of obstacle at the specified coordinates
6. If there is no obstacle, turtlebot reaches the location and notifies you
7. Open a new terminal and run,
        roslaunch turtlebot_rviz_launchers view_navigation.launch
   to view simulation in rviz