# turtlebot_follower
## Dependencies
- Ubuntu 16.04
- gazebo 7
- ROS Kinetic
- Catkin
- roscpp package
- turtlebot package
## To build
```
$ sudo apt-get update
$ sudo apt-get upgrade

$ wget https://raw.githubusercontent.com/ROBOTIS-GIT/robotis_tools/master/install_ros_kinetic.sh
$ chmod 755 ./install_ros_kinetic.sh 
$ bash ./install_ros_kinetic.sh
$ sudo apt-get install ros-kinetic-joy ros-kinetic-teleop-twist-joy \
  ros-kinetic-teleop-twist-keyboard ros-kinetic-laser-proc \
  ros-kinetic-rgbd-launch ros-kinetic-depthimage-to-laserscan \
  ros-kinetic-rosserial-arduino ros-kinetic-rosserial-python \
  ros-kinetic-rosserial-server ros-kinetic-rosserial-client \
  ros-kinetic-rosserial-msgs ros-kinetic-amcl ros-kinetic-map-server \
  ros-kinetic-move-base ros-kinetic-urdf ros-kinetic-xacro \
  ros-kinetic-compressed-image-transport ros-kinetic-rqt* \
  ros-kinetic-gmapping ros-kinetic-navigation ros-kinetic-interactive-markers``

$ sudo apt-get install ros-kinetic-dynamixel-sdk
$ sudo apt-get install ros-kinetic-turtlebot3-msgs
$ sudo apt-get install ros-kinetic-turtlebot3

$ cd ~/catkin_ws/
$ catkin_make
$ cd ~/catkin_ws/src
$ git clone https://github.com/Kemojiji/turtlebot_follower.git
$ cd ~/catkin_ws/
$ catkin_make
````
## To run
The following command starts the gazebo world with keyboard to control the first robot 
```
$ roscore
$ source devel/setup.bash
$ roslaunch turtlebot_follower turtlebot_follower.launch
```
## Viedo
(https://youtu.be/USkKm8jqA9A)
## Ensure the code is working 
- Double check the dependencies
- Source the environemnt befor roslaunch 
- I will frequently update the this github repository if i made change on my local machine
- The next step can be use Docker to deploy it. Docker is a virtualization technique that packages the entire code and the environment, then deploys the applications on a different local machine without sharing any OS or system-level resources.
