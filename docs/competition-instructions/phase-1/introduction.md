# Introduction

## Navigation Challenge

<!-- Nav2 -->

The simulation platform to be used in this track is [Gazebo Harmonic](https://gazebosim.org/docs/harmonic/install_ubuntu/). Teams are required to develop, test and submit software to successfully complete the task of autonomously navigating the **CAYTU Sito-É** through maize fields. 

Teams are provided with the **CAYTU Sito-É**'s ROS 2 packages and Gazebo environment models (see description below) to enable them develop and test their solutions (see [GitHub Repository](https://github.com/PARC-Robotics/PARC2026-Engineers-League)).

### The CAYTU Sito-É

The **CAYTU Sito-É** is an unmanned ground vehicle (UGV) equipped with different sensors to help you achieve your goal. The sensors are:

* **RPLIDAR C1:** A LiDAR sensor located at the top of the base of the robot. The RPLIDAR C1 publishes the `/scan` topic.

* **D435i Camera (x2):** Two side-facing RGB cameras are provided at the left and right side of the robot. These cameras are suspended via an overhang and gives top-view of the farmland. The topics published by these cameras have group names which are `/top_camera/` and `/right_camera/`.

<!-- The depth blah blah -->

<!-- * **ZED 2i Camera:** This is a stereo camera at the front of the robot base. It publishes all the `/zed2/` topics including point cloud data(`/zed2/point_cloud/cloud_registered`) -->

* **IMU:** An IMU sensor is added to the base and publishes on the `/imu` topic.

The figure below shows the Sito-É with the sensors labelled.

![robot](../assets/robot_sensor_label.png)


<!-- ### Simulation Environment

The simulation environment used in this phase is modeled as a realistic farmland with rough terrain and maize plants and was generated with the [virtual maize field](https://github.com/FieldRobotEvent/virtual_maize_field) ROS package.

![simulation](../assets/world_description.png) -->

<!-- This phase will evaluate the teams' capabilities to successfully complete these fundamental tasks required to compete in phase 2 (on the physical robot). -->