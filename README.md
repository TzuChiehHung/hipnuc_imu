# hipnuc_imu

Forked from [hipnuc/products](https://github.com/hipnuc/products)

A ROS package for HiPNUC HI226/Hi229 IMU Device.

## Install dependencies

```bash
sudo apt install ros-$ROS_DISTRO-serial
sudo apt install ros-$ROS_DISTRO-geometry-msgs
```

## Change permission

create file `/etc/udev/rules.d/70-ttyusb.rules`:
```bash
KERNEL=="ttyUSB[0-9]*",MODE="0666"
```

## Launch

```bash
roslaunch hipnuc_imu imu.launch
```