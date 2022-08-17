# Task-1-2
This file presents the steps for installing 'ROS' into Ubuntu.

1. Setup Ubuntu repositories:

sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'


2. Setup the keys:


sudo apt install curl
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -


3. Installation:

sudo apt update

Desktop-Full Install: 
sudo apt install ros-noetic-desktop-full

Desktop Install: 

sudo apt install ros-noetic-desktop


ROS-Base: (Bare Bones) ROS packaging, build, and communication libraries. No GUI tools.

sudo apt install ros-noetic-ros-base

when we want to install a certtain package we should use this command:


sudo apt install ros-noetic-PACKAGE NAME

for finding other available packages, we use:
apt search ros-noetic

4. Setup the enviroment

source /opt/ros/noetic/setup.bash

5. Dependencies for building packages

For installing tool and other dependencies for building ROS packages:

sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential

5.1. Initialize rosdep

sudo apt install python3-rosdep
Initialize rosdep and update it

sudo rosdep init
rosdep update
