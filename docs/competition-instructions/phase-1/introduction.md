# Introduction

## Navigation Challenge

<!-- Nav2 -->

The simulation platform to be used in this challenge is [Gazebo Harmonic](https://gazebosim.org/docs/harmonic/install_ubuntu/). Teams are required to develop, test and submit software to successfully complete the task of autonomously navigating the **CAYTU Sito-É** in the restaurant, from its start position to the goal position. 

## Vision Challenge
In progress

Teams are provided with the **CAYTU Sito-É**'s ROS 2 packages and Gazebo environment models (see description below) to enable them develop and test their solutions (see [GitHub Repository](https://github.com/PARC-Robotics/PARC2026-Engineers-League)).

### The CAYTU Sito-É

The **CAYTU Sito-É** is an unmanned ground vehicle (UGV) equipped with different sensors to help you achieve your goal. The sensors are:

* **RPLIDAR C1:** A LiDAR sensor located at the top of the base of the robot. The RPLIDAR C1 publishes on the `/scan` topic.

* **D435i Depth Camera (x2):** One camera is mounted below the monitor the robot and the other towards the robot's base. These cameras publish color data on the topics `/top_camera_color/image_raw` and `/bottom_camera_color/image_raw` and 3D point cloud data on `/top_camera_depth/points` and `/bottom_camera_depth/points`. There are also topics for compressed images which use lower bandwidth compared to the standard raw image. Considering the top D435i camera, these topics are `/top_camera_color/image_raw/compressed` and `/top_camera_color/image_raw/theora`, with similar topics available for the bottom D435i camera as well.

* **IMU:** An IMU sensor is added to the base and publishes on the `/imu` topic.

The figure below shows the Sito-É with the sensors labelled.

![robot](../assets/robot_sensor_label.png)


<!-- ### Simulation Environment

The simulation environment used in this phase is modeled as a realistic farmland with rough terrain and maize plants and was generated with the [virtual maize field](https://github.com/FieldRobotEvent/virtual_maize_field) ROS package.

![simulation](../assets/world_description.png) -->

<!-- This phase will evaluate the teams' capabilities to successfully complete these fundamental tasks required to compete in phase 2 (on the physical robot). -->