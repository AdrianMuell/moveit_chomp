# Wiki

## LogGPIS-ROS
1. start roscore <br>
```
roscore
```
2. start LogGPIS <br>
```
rosrun gpismap_ros gpismap3
```
3. run rosbag <br>
```
rosbag play <rosbag_name>
```
4. starting moveit without real Robot <br>
```
roslaunch ur5e_moveit_config demo.launch pipeline:=chomp
```
5. start rqt and call service "/reset_traj_pts" <br>
```
roslaunch ur5e_moveit_config demo.launch pipeline:=chomp
```
6. moving robot to joint goals
```
rosrun gpismap_ros move_ur5e
```
## Gazebo
1. start gazebo with scene
(change scene in )
```
roslaunch gazebo-depth-sim gazebo.launch
roslaunch gazebo-depth-sim gazebo.launch world_name:=<world_path>
```
2. start Tool for playing and collecting Camera Movements
```
rosrun gazebo-depth-sim position_control_cam_gazebo
```