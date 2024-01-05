# RoboSense Helios ROS 2 Interface

## Introduction
This repository contains ROS 2 packages designed to interface with the RoboSense 32-layer Helios LiDAR. These packages allow for the conversion of RoboSense data to Velodyne data formats.

## Dependencies
To ensure proper functionality of the packages, the following dependencies are required:
### pcl_conversions (Essential) 

### Yaml (Essential) 

version: >= v0.5.2

Installation:

```sh
sudo apt-get update
sudo apt-get install -y libyaml-cpp-dev
```

### libpcap (Essential) 

version: >= v1.7.4

Installation:

```sh
sudo apt-get install -y  libpcap-dev
```


## How to Use

After compiling the packages, you can launch the nodes to interface with the RoboSense LiDAR in the ROS 2 environment.

### For RoboSense Data Format
To run the node that interfaces with the RoboSense data format, use the `start.py` launch file:

```sh
ros2 launch rslidar_sdk start.py
```

### For Velodyne Data Format
If you need to work with the Velodyne data format, execute the velodyne.py launch file instead:

```sh
ros2 launch rslidar_sdk velodyne.py
```
