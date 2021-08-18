# GazeboArm
Gazebo simulation of a robot arm picking up a ball and dropping it into a bucket

Installation:
1. Install anaconda3
2. Update your C++ compiler to latest version (e.g. glibc)
3. Create anaconda package with python=3.8
4. Install gcc_linux-64 version 11.1.0 through conda-forge
5. Follow installation instructions for ros-noetic
6. Git clone arbotix_ros and pincher_arm repositories into catkin_ws/src
7. (From catkin_ws directory now) rosdep install --from-paths src --ignore-src -r -y
9. catkin_make
10. Add ROS_HOSTNAME and ROS_MASTER_URI env variables to .bashrc

Running The Simulation:
1. Open another terminal window and run roscore
2. export ROS_PACKAGE_PATH=/home/myusername/catkin_ws/src:$ROS_PACKAGE_PATH
3. rosparam set use_sim_time true

Links:
- https://github.com/RoboStack/ros-noetic
- https://github.com/vanadiumlabs/arbotix_ros
- https://github.com/fictionlab/pincher_arm
- http://gazebosim.org/tutorials/?tut=ros_urdf
