# How to Submit

Teams are expected to develop their solutions (ROS packages) in a 'solutions' folder inside the `~/ros2_ws/src` directory. You may have one or more ROS packages in this folder. 

This is the expected directory structure:

```
~/ros2_ws/src
.
├── parc_robot
│   ├── CMakeLists.txt
│   └── package.xml
├── parc_robot_bringup
│   ├── .
│   ├── .
│   ├── CMakeLists.txt
│   └── package.xml
├── parc_robot_description
│   ├── .
│   ├── .
│   ├── CMakeLists.txt
│   └── package.xml
├── .
├── .
└── <YOUR_SOLUTION_FOLDER>        # Zip this folder and submit
    ├── <your_ros_package1>
    │   ├── .
    │   ├── .
    │   ├── setup.py
    │   └── package.xml
    ├── <your_ros_package2>
    │   ├── .
    │   ├── .
    │   ├── setup.py
    │   └── package.xml
    ├── .
    ├── .
    └── README.md                   # Required
```

Follow these submission steps:

1. Prepare a README.md file following this format and store in solution folder (see [example](https://github.com/PARC-Robotics/PARC2026-Engineers-League/blob/main/resources/sample-submission-readme.md)):
    * Introduction Section: Briefly describe your approach
    * Dependencies: List all the packages installed and used in your solution
    * Task description and run command(s)
    * Challenges faced

2. Include all the packages (dependencies) used in your solution in your package's "package.xml" file ([see guide](https://docs.ros.org/en/jazzy/Tutorials/Intermediate/Rosdep.html){target=_blank})

3. Create simple short video demos of your solution. This can be done by taking a screen recording of your solution running in Gazebo. Please ensure the videos are less than 200 MB in size.

4. Zip your solution folder and upload the folder and the videos on the solution submission form (TO BE PROVIDED).

<!-- 4. Zip your solution folder and upload the folder and the videos on the [solution submission form](https://forms.gle/GwE7Tzm9FpYzUVQX9). -->