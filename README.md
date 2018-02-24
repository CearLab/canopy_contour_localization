# canopy_contour_localization

## Setup
```
mkdir -p canopy_contour_localization_ws/src
cd canopy_contour_localization_ws/src
catkin_init_workspace
clone https://github.com/CearLab/canopy_contour_localization
cd ..
catkin_make
source devel/setup.bash
```

## Running experiments
Copy the relevant bag file
```
roslaunch contour_based_localization global_localization_comparison.launch
rosbag play <name_of_bag.bag>
```

## Data
Available in https://drive.google.com/open?id=1pcCh1iWMyDpUokzW0wuFARI15O9Fz3SG
