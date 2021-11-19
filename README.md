# Adaptive_MCL

## Adaptive Monte-Carlo Localisation ##
is a probabilistic localization system for a robot moving in 2D. It implements the adaptive (or KLD-sampling) Monte Carlo localization approach (as described by Dieter Fox), which uses a particle filter to track the pose of a robot against a known map. (Source amcl - ROS WIKI)

## Build Steps ##
#### 1. Clone The Repository ####
```
git clone https://github.com/Iaryan-21/Adaptive_MCL
```
#### 2. Build the file ####
```
source devel/setup.bash
```
#### 3. Launch world node ####
```
roslaunch my_robot world.launch
```
#### 4. Launch amcl node ####
```
roslaunch my_robot amcl.launch
```
#### 5. Go to RVIZ , open the file> open file> launch file (in repository)> my_robot_config.launch ####

### OPTIONAL ###
#### 6. Run the teleop node ####
```
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

### IMPORTANT ###

*The above file is also added in the repository, if one does not intend to use the teleop node, one can goto 2D estimate on RVIZ to assign direction for the movement of the robots*

*In maps folder, extract the .zip folder to the maps folder itself and delete the .zip file*
