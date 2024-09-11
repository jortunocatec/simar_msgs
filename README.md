# SIMAR Messages
This repository contains the definition of the ROS messages used in the SIMAR project.

## Installation
This package is tested under [ROS Noetic](https://wiki.ros.org/noetic/Installation/Ubuntu) and Ubuntu 20.04.
To install the messages in your workspace, clone the repository and build it using catkin_make.

## Messages description
The following table describes the messages defined in this package.

| Message name | Description |
| ------------ | ----------- |
| [simar_msgs/Alarm](msg/Alarm.msg) | Message used to send alarms to the system. |
| [simar_msgs/PayloadAction](msg/PayloadAction.msg) | Message used to send actions to the availble payloads. |
| [simar_msgs/ExtremeTemps](msg/ExtremeTemps.msg) | Message used to publish the extreme temperature data.|
| [simar_msgs/PixelTemp](msg/PixelTemp.msg) | Message used to show the temperature of a pixel. |


## Services description
The following table describes the services implemented in SIMAR packages.

### USE Packages

| Services name | Description |
| ------------- | ----------- |
| `connectServiceCB` | Connects to the camera. |
| `captureServiceCB` | Captures an image. |
| `recordingStartServiceCB` | Starts video recording. |
| `recordingStopServiceCB` | Stops video recording. |
| `zoom(int)` | Controls zoom for thermal and visible cameras. |
| `zoomInServiceCB` / `zoomOutServiceCB` | Controls camera zoom. |
| `setEthStreamServiceCB` / `getEthStreamServiceCB` |  Manages Ethernet stream service. |
| `getExtTempServiceCB` | Gets the extreme temperature data from the camera. |


