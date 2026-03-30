# Mobile Robotics Platform
Mobile Robotics Platform running on ROS2, capable of running SLAM and autonomously navigating a space.

A combination of low-level C microcontroller code, electrical design, 3D-printing, low-level C++ custom ROS2 nodes and high-level Python scripts.

## New version in-progress
Once complete, this repo will be updated with more media.

## Physical Specifications
- Small form factor: 20cm diameter circle footprint
- 3D printed housing with levels to house each
- Custom PCB in the works that integrates ESP32-S3-WROOM-1 with DRV8871 motor drivers to connect with 12V system and one JST connector per motor for ease of wiring
  - In progress. Current version uses breakout board versions of the components
- Custom 3S2P 18650 battery in the works
- Utilizes ESP32 for low-level operations, such as driving motors or calculating motor velocities
- Raspberry Pi 5 16GB runs Ubuntu 24.04 with ROS 2 Jazzy
- YDLIDAR G4 for LiDAR localization and mapping
- RealSense D435 for obstacle detection
## Tech Specs
- ROS2 Jazzy, running under Ubuntu 24.04 with real-time kernel
- Utilizing realsense-ros node and ydlidar_ros2_driver
  - In progress: Custom-built node to interface with ESP32. Current version uses Josh Newan's code to communicate with Arduino
- Nav2 node used for navigating between points
- slam_toolbox used for mapping
