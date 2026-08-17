#  Simulated Cave Environments - DARPA Subterranean Challenge

ROS 2 data package containing subterranean environments for Gazebo Sim. It can
be built and used as a standalone repository and has no nodes or runtime ROS
dependencies.

## Included worlds

| World | Environment |
| --- | --- |
| `darpa_cave_01.sdf` | DARPA SubT cave circuit and default UAV simulation world |
| `darpa_cave_02.world` | Alternate cave circuit with artifacts |
| `darpa_cave_03.world` | Alternate cave circuit with vertical sections |
| `niosh_osrf.world` | NIOSH mine environment |
| `pittsburgh_mine.sdf` | Pittsburgh mine mesh |
| `urban_circuit_01.sdf` | DARPA SubT urban circuit |

All models required by these worlds are installed with the package under
`share/subt_cave_sim/models`.

## Prerequisites

- ROS 2 with `ament_cmake` and `colcon`
- Gazebo Sim (`gz sim`)

## Build in a ROS 2 workspace

Place this repository in the `src` directory of a ROS 2 workspace, then run:

```bash
source /opt/ros/$ROS_DISTRO/setup.bash
cd /path/to/your/workspace
colcon build --packages-select subt_cave_sim --symlink-install
source install/setup.bash
```

## License

The simulation models are sourced from Open Robotics Fuel and licensed under
the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
See [LICENSE](LICENSE) for attribution details.
