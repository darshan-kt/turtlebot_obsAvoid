## TurtleBot3 Obstacle Avoidance Simulation

The turtlebot_obsAvoid package provides a complete simulation setup for testing obstacle avoidance using the TurtleBot3 robot in a Gazebo environment. It utilizes ROS navigation stack with move_base and is compatible with the waffle_pi model of TurtleBot3.
#### Package Features

    Supports TurtleBot3 Waffle Pi model

    Launches a simulated environment in Gazebo

    Uses the ROS Navigation Stack (move_base) for autonomous movement

    Integrates sensor data for real-time obstacle avoidance

    Simple to launch and test from terminal

### Setup & Launch Instructions
Set the TurtleBot3 model:
```bash
export TURTLEBOT3_MODEL=waffle_pi
```
Launch the Gazebo simulation:

```bash
roslaunch turtlebot3_gazebo sim.launch
```
Start the navigation stack with obstacle avoidance:
```bash
roslaunch turtlebot3_navigation move_base.launch
```
### Navigation with Rviz

Once the simulation and navigation stack are running:

    Open Rviz (should launch automatically).

    Use the "2D Nav Goal" tool to set a destination.

    The TurtleBot3 will plan and navigate around obstacles using laser scans and the move_base planner.
