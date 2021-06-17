# iRobot Create 3

[![Linter](https://github.com/iRobotSTEM/create3_sim/actions/workflows/lint.yml/badge.svg)](https://github.com/iRobotSTEM/create3_sim/actions/workflows/lint.yml) [![Testing](https://github.com/iRobotSTEM/create3_sim/actions/workflows/ci.yml/badge.svg)](https://github.com/iRobotSTEM/create3_sim/actions/workflows/ci.yml) [![License](https://img.shields.io/github/license/iRobotSTEM/create3_sim)](https://github.com/iRobotSTEM/create3_sim/blob/master/LICENSE)

This is a [ROS 2](https://docs.ros.org/en/foxy/index.html) simulation stack for the [iRobot Create 3]() robot.

## Prerequisite

Before moving forward make sure to have either ROS foxy or ROS galactic installed. 

## Build

- Create a workspace if you don't already have one:

```bash
mkdir -p ~/colcon_ws/src
```

- Clone this repository into the src directory from above.

- Navigate to the workspace and install ros2 dependencies with:

```bash
cd ~/colcon_ws
rosdep install --from-path src -yi
```

- Build the workspace with:

```bash
colcon build --symlink-install
source install/local_setup.bash
```

## Examples

Create 3 can be spawned in an empty world in RViz with

```bash
ros2 launch irobot_create_description rviz2.launch.py
```

## [Contributions](CONTRIBUTING.md)