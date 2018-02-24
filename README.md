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

## Data Preparation
Get data from https://drive.google.com/open?id=1pcCh1iWMyDpUokzW0wuFARI15O9Fz3SG
1. Generate canopies and trunks bags using contour_based_localization/scripts/utils/image_to_bag.py
2. Merge pose bags with canopies and trunks bags using contour_based_localization/scripts/utils/merge_bags.py


## Experiments
```
roslaunch contour_based_localization global_localization_comparison.launch
rosbag play <name_of_merged_bag.bag>
```
