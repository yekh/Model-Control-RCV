# Memo

This file contains a record of useful stuffs about this project in case we forget.

### camera view (close)

<pose>4.5 -22 3.48 0 0.24 1.63</pose>

### original initial parameters

torque 859.4004393000001

braketorque 687.5203514400001

### check RCV state from Gazebo

```
$ rostopic echo /base_pose_ground_truth
```

### launch planning-path visualizer

```
$ cd catkin_ws
$ catkin_make
$ roslaunch run_sim run_sim.launch
```

in a new terminal

```
$ roslaunch move_base_config move_base.launch
```

in a new terminal

```
$ rosservice list |grep  file (could skip)
$ rosservice call /load_path_from_file "path_filename: '/home/el2425/catkin_ws/src/simulation_nodes/fake_planning/path_from_file_planner/data/path.dat' 
> ignore_heading: false"
```

in rviz, add -> path

### road width

checked coordinates of the car at both sides of the road (~14 m), which corresponds to the width of a 4-lane highway.
