# Autonomous-Warehouse-Navigation

This project contains a complete simulation setup for a mobile robot in a warehouse environment using ROS and Gazebo. It includes SLAM, localization, navigation, and URDF-based robot description.

## 📁 Project Structure

```
Final/
├── launch/                  # ROS launch files for various components
├── meshes/                  # 3D model files (e.g., sensors)
├── urdf/                    # Robot URDF and xacro descriptions
├── model/                   # Gazebo model configuration files
├── Map/                     # Predefined map (YAML and PGM)
└── worlds/                  # Gazebo world file
```

## 🚀 Launch Instructions

Make sure you have ROS (preferably Noetic) installed and sourced.

```bash
cd Final
roslaunch launch/world.launch             # Launch the Gazebo world
roslaunch launch/robot_description.launch # Load robot description
roslaunch launch/gmapping_demo.launch     # Run SLAM using Gmapping
roslaunch launch/localization.launch      # Run localization (AMCL)
roslaunch launch/navigation.launch        # Start move_base navigation
```

## 🧰 Dependencies

- ROS (Noetic)
- Gazebo (compatible with your ROS version)
- `gmapping`, `amcl`, `move_base`, and other navigation stack packages

## 🗺️ Map

The map is located in the `Map/` directory and is used for localization and navigation.

## 🧪 World

The custom Gazebo world is defined in `worlds/Warehouse1.world`.

---

Feel free to fork, contribute, or use this setup for mobile robot simulations.
