# ROS Vagrant Virtual Machines

Vagrant Virtual Machines for multiple versions (and combinations of versions) of ROS and Ubuntu:

- Provision Ubuntu virtual machines with GUI (to run Gazebo and other visualization tools)
- Loads a synced folder to share code from host machine to guest virtual machine. The synced folder in host is inside
  the relevant version folder and in the guest machine, you can find the folder at the path `/home/ros_ws`

## Requirements

1. [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
2. [Vagrant](https://www.vagrantup.com/downloads.html)

## Instructions

1. Get on the folder with versions you want to run e.g. `cd melodic-bionic`
2. Provision the virtual machine by running `vagrant up`
3. You can then start the graphical environment by starting the machine from the VirtualBox program or
   start a non-gui session by running the command `vagrant ssh`. If you sign in from the GUI then use the following default vagrant credentials:
   username: **vagrant** and password **vagrant**
4. To delete a machine completely, go to the VirtualBox program, find the VM and click on delete all files and then on
   this folder delete the `.vagrant` folder.

## Version Matrices

### Ubuntu x64 vs ROS

|             |         Focal <br> (20.04 LTS)          |         Bionic <br>(18.04 LTS)          | Zesty <br>(17.04) |         Xenial <br>(16.04 LTS)          | Trusty <br>(14.04 LTS) | Precise <br>(12.04 LTS) |
| :---------: | :-------------------------------------: | :-------------------------------------: | :---------------: | :-------------------------------------: | :--------------------: | :---------------------: |
| **Melodic** | [Supported](./melodic-focal/README.md) | [Supported](./melodic-bionic/README.md) |
|  **Lunar**  |                                         |                                         |                   |  [Supported](./lunar-xenial/README.md)  |
| **Kinetic** |                                         |                                         |                   | [Supported](./kinetic-xenial/README.md) |
|  **Jade**   |                   EOL                   |                   EOL                   |        EOL        |                   EOL                   |          EOL           |           EOL           |
| **Indigo**  |                   EOL                   |
|  **Hydro**  |                   EOL                   |                   EOL                   |        EOL        |                   EOL                   |          EOL           |           EOL           |
| **Groovy**  |                   EOL                   |                   EOL                   |        EOL        |                   EOL                   |          EOL           |           EOL           |

### Ubuntu x64 vs ROS 2

|             |         Bionic <br>(18.04 LTS)          | Zesty <br>(17.04) |         Xenial <br>(16.04 LTS)          | Trusty <br>(14.04 LTS) | Precise <br>(12.04 LTS) |
| :---------: | :-------------------------------------: | :---------------: | :-------------------------------------: | :--------------------: | :---------------------: |
| **Crystal** | [Supported](./crystal-bionic/README.md) |                   | [Supported](./crystal-xenial/README.md) |
| **Bouncy**  | [Supported](./bouncy-bionic/README.md)  |                   | [Supported](./bouncy-xenial/README.md)  |

### Gazebo vs ROS versions

In the Vagrant boxes of this repository the Recommended versions for Gazebo are installed (TODO)

|             |    Gazebo 9     | Gazebo 8  |    Gazebo 7     |    Gazebo 2     |
| :---------: | :-------------: | :-------: | :-------------: | :-------------: |
| **Melodic** | **Recommended** |           |                 |                 |
|  **Lunar**  |    Supported    | Supported | **Recommended** |                 |
| **Kinetic** |    Supported    | Supported | **Recommended** |                 |
| **Indigo**  |                 |           |    Supported    | **Recommended** |
