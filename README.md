# Run Instructions

```
# Terminal 1
$ source ~/gecko_ws/devel/setup.bash
$ roscore

# Terminal 2
$ source ~/gecko_ws/devel/setup.bash
$ roslaunch openni_launch openni.launch

# Terminal 3
$ source ~/gecko_ws/devel/setup.bash
$ rosrun pcproxy pcproxy

# Terminal 4
$ source ~/gecko_ws/devel/setup.bash
$ rosrun showpc showpc
```

# Installation

## Prerequisites

### Ubuntu 14.04
Install Ubuntu 14.04 on your computer. You can get the .iso from [this website](http://releases.ubuntu.com/14.04/).

### ROS Indigo
Install ROS Indigo on your computer. You can find installation instructions [here](http://wiki.ros.org/indigo/Installation/Ubuntu).

### Create a Workspace
In order to install this repository's code, as well as the camera driver, you need to create a Workspace.

```
$ sudo apt-get install python-catkin-tools
$ cd ~
$ mkdir gecko_ws
$ cd gecko_ws
$ mkdir src
$ catkin init
```

### Openni V1 ROS Driver for Kinect V1
# Openni for Kinect V1 (Works)

To install ([Original Instructions](blog.justsophie.com/installing-kinect-nite-drivers-on-ubunut-14-04-and-ros-indigo)):

```
$ sudo apt-get install libopenni0 libopenni-dev
$ cd ~/gecko_ws/src
$ git clone https://github.com/ros-drivers/openni_launch.git
$ git clone https://github.com/ros-drivers/openni_camera.git
$ catkin build
```

See above for the commands to run the driver.

## gecko_foyer

```
$ cd ~/gecko_ws/src
$ git clone https://github.com/wrobotics/gecko_foyer.git
$ catkin build
```