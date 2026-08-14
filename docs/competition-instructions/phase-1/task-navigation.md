# Navigation Task

## General Description

<!-- ![task1_simulation](../assets/task_sim.gif) -->

An autonomous service robot operating in a stadium should be capable of performing numerous functions with one of the most fundamental being autonomous navigation. The robot should be able to perceive its surroundings with its sensors, in order to detect crowds and obstacles, plan a path around them, follow that trajectory and making adjustments when crowds or obstacles change. Teams must develop a software solution using [Nav2](https://docs.nav2.org/index.html){target=_blank} that guides the robot from its starting position to its goal location.

<!-- Add gif of the robot moving around, mention that the actors won't interfere -->

## Task Guidelines

### Launching the Task
In a new terminal, run the following launch file to bring up the robot in Gazebo and RViz:

```sh
ros2 launch parc_robot_bringup task.launch.py
```

You should see the display below in Gazebo and RViz respectively. The robot is in the middle and towards the top left is the green circle which represents the goal location.

=== "Gazebo"
    ![task1_gazebo](../assets/gazebo.png)

=== "RViz"
    ![rviz](../../getting-started-tutorials/assets/rviz.png)

### Preparing your Solution
* Your solution should be prepared as ROS packages to be saved in your solution folder. Create a node executable file in your ROS package which runs ALL the code you need in your solution. Name this node file: `task_solution.py`.

* Hence, your solution should be run by calling the following commands:

In one terminal:

```sh
ros2 launch parc_robot_bringup task.launch.py
```

!!! note "Note"
    Please wait until both the world and robot models have finished spawning. This process may take longer than usual, especially when running the program for the first time.

In another terminal:

```sh
ros2 run <your-package-name> task_solution.py>
```

Launch files can also be used in your solution.

## Task Rules

* The time limit to complete the task is **10 minutes (600 seconds)**.

* The task is ONLY complete when ANY part of the robot is inside the green circle (goal location marker).

## Autonomy Evaluation

Scoring for this task would be based on the following criteria:

| S/N      | Criteria/Metric | Description |
| ----------- | ----------- | ------- |
| 1  | **Obstacle avoidance**  | The robot should avoid making contact with any obstacles. **(Less contact is better)** |
| 2 | **Final travel distance to goal** | Shortest travel distance from robot (measured from robot center) to the goal which is calculated at the time limit [10 minutes] **(Smaller is better)**
| 3  | **Completion time** | Time from launching the solution to task completion **(Smaller is better)** |
