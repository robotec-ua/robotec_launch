# Agrotec Robot Launch Package
This is the package dedicated to start all the system of Robotec packages. All the parameters are stored here, so the packages doesn't need to be configurated.

## Table of contents
* [Project structure](#project_structure)
    * [Folders](#folders)
    * [Files](#files)
* [Usage](#usage)

## Project structure
```
.
├── config
│   └── robotec_velocity_controller
│       └── diff_drive_controller.yaml
├── launch
│   ├── gmapping
│   │   └── gmapping.launch
│   ├── pid
│   │   └── pid.launch
│   ├── robotec_launch
│   │   └── robotec_launch.launch
│   ├── robotec_move_basic
│   │   └── robotec_move_basic.launch
│   ├── robotec_mrcnn
│   │   └── robotec_mrcnn.launch
│   ├── robotec_odom_publisher
│   │   └── robotec_odom_publisher.launch
│   ├── robotec_velocity_controller
│   │   └── robotec_velocity_controller.launch
│   ├── robot_localization
│   │   └── robot_localization.launch
│   ├── robot_pose_publisher
│   │   └── robot_pose_publisher.launch
│   ├── rosserial_python
│   │   └── rosserial_python.launch
│   └── tf2
│       └── tf2.launch
├── param
│   ├── imu
│   │   └── imu_calibration.yaml
│   ├── move_basic
│   │   └── move_basic.yaml
│   ├── robotec_mrcnn
│   │   └── robotec_mrcnn.yaml
│   └── robot_localization
│       └── robot_localization.yaml
├── CMakeLists.txt
├── LICENSE
├── package.xml
├── README.md
└── TODO.md
```

### Folders
* `launch` : ROS launch files
* `param` : configuration parameters files
* `config` : configuration files of packages

### Files
* `CHANGELOG.md` : the file where the changes to the project are desribed
* `README.md` : the documentation of the project
* `TODO.md` : suggesting changes in the package 
* `launch/<package_name>/<package_name>.launch` : launching <package_name> with desired parameters
* `param/<package_name>/<package_name>.yaml` : desired parameters for <package_name>
* `imu_calibration.yaml` : calibration parameters for the IMU, used in Robotec products (MPU9250)
* `diff_drive_controller.yaml` : configuration file for diff_drive_controller (part of ros_controllers)  

## Usage
Everything you need to start the whole robot is to run the command :
```bash
$ roslaunch agrotec_launch agrotec_launch/agrotec_launch.launch
```
