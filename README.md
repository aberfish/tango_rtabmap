# tango_rtabmap
ROS package using rtabmap to construct maps from sensor data, configured for the tango robot

## Setup:
Place the contents of this repository in the directory:
```<path_worksapce_dir>/src/tango_rtabmap```

Build and source your ROS workspace:
```cd <path_to_workspace_dir>```, 
```catkin_make```, 
```source devel/setup.bash```

## Current usage:
This package currently only contains a utility to construct a map from a collected rosbag containing topics ```/odom``` and ```/scan```

```roslaunch tango_rtabmap tango_rtabmap_bag_mapping bag:=<path_to_bagfile>/<filename>.bag```
