# diff_car

# First run the robot use any of the launch files
roslaunch diff_car robot_world.launch

# Launch Rviz

rosrun rviz rviz

# Create map using
rosrun gmapping slam_gmapping scan:=scan 

### Make sure that reference frame is odon on rviz

# Save Map using
rosrun map_server nap_saver 'name'

# launch move_base node

roslaunch diff_car move_base.launch

### make sure to change the reference frame to map on rviz ###

