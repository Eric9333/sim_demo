# sim_demo

This package contains a simple four-wheel robot for Gazebo simulation.  An obstacle world and a launch file for laser SLAM are provided.

## Usage

```bash
roslaunch sim_demo lidar_mapping.launch
```

This spawns the robot in `obstacle_world.world` and runs `slam_gmapping` to build a map from the lidar topic `/simple_scan`.
