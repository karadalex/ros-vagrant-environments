ROS Vagrant Virtual Machines
============================

Vagrant Virtual Machines for multiple versions (and combinations of versions) of ROS and Ubuntu

## Requirements

1. [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
2. [Vagrant](https://www.vagrantup.com/downloads.html)


## Version Matrices


### Ubuntu x64 vs ROS

|             | Bionic <br>(18.04 LTS) | Zesty <br>(17.04) | Xenial <br>(16.04 LTS) | Trusty <br>(14.04 LTS) | Precise <br>(12.04 LTS) |
| :---------: | :--------------------: | :----------------: | :--------------------: | :--------------------: | :---------------------: |
| **Melodic** | [Supported](./melodic-bionic/README.md) |
| **Lunar**   |  |  | [Supported](./lunar-xenial/README.md) |
| **Kinetic** |  |  | [Supported](./kinetic-xenial/README.md) |
| **Jade**    | EOL | EOL | EOL | EOL | EOL |
| **Indigo**  |
| **Hydro**   | EOL | EOL | EOL | EOL | EOL |
| **Groovy**  | EOL | EOL | EOL | EOL | EOL |

### Ubuntu x64 vs ROS 2

|             | Bionic <br>(18.04 LTS) | Zesty <br>(17.04) | Xenial <br>(16.04 LTS) | Trusty <br>(14.04 LTS) | Precise <br>(12.04 LTS) |
| :---------: | :--------------------: | :----------------: | :--------------------: | :--------------------: | :---------------------: |
| **Crystal** | [Supported](./crystal-bionic/README.md) |  | [Supported](./crystal-xenial/README.md) |
| **Bouncy**  | [Supported](./bouncy-bionic/README.md) |  | [Supported](./bouncy-xenial/README.md) |

### Gazebo vs ROS versions

In the Vagrant boxes of this repository the Recommended versions for Gazebo are installed (TODO)

|         |  Gazebo 9   |  Gazebo 8   |  Gazebo 7   |  Gazebo 2   |
| :-----: | :---------: | :---------: | :---------: | :---------: |
| **Melodic** | **Recommended** |             |             |             |
| **Lunar**   | Supported   | Supported   | **Recommended** |             |
| **Kinetic** | Supported   | Supported   | **Recommended** |             |
| **Indigo**  |             |             | Supported   | **Recommended** |