# Repository for VT2 - Capra Robotics

## Setup for dummies
Go to the folder you want to place your workspace in (e.g. home)
```
source /opt/ros/galactic/setup.bash
```
1. create new directory
```
mkdir -p ~/VT2_ws/src
cd ~/VT2_ws/src
```
2. Clone CapraVT2 repository
```
git clone https://github.com/ros/ros_tutorials.git
```
3. Resolve dependencies (go to root of the workspace first "VT2_ws")
```
cd ..
rosdep install -i --from-path src --rosdistro galactic -y
```
4. Build the workspace
```
colcon build
```