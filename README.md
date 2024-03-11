# Raspberry Pi 4 and RPLIDAR in ROS Noetic 🤖

ROS is Robot Operating System which allow us to create robotic systems and to communicate components each oether in robots.  This project shows us how to use ROS to show RPLIDAR data in RVIZ. All system developed by using Raspberry Pi 4+ 8GB. 
<br/><br/>
<img src="https://github.com/gorselanaliz/raspberry_pi_rplidar_ros/blob/main/project.avif" width="500">

## Getting Started

These instructions will show you how to run and visualize RPLIDAR data on your Raspberry Pi for development and testing purposes. This repo is for visualizing RPLIDAR data on RVIZ but you can easily implement HectorSlam on your system. This project consist of 2 steps:

* Raspberry Pi and RPLIDAR Handeld Kit Design 
* RPLIDAR Data Visualization on Raspberry Pi in ROS Noetic
<br/>

![]()
<br/>


## Prerequisites

Ubuntu 20.04 and ROS Noetic should have been installed on your Raspberry Pi. This means that we are not going to use Raspian Operating System in this project.

Software:
* ROS Noetic
* Ubuntu 20.04
* RPLIDAR ROS Package
  
Hardware:
* RPLIDAR A1M8
* Raspberry Pi 3/4/5
* 5V & 2.5/3A Powerbank
* Handheld Kit (not necessary) 

<br/>

## Installation

A step by step guide that will tell you how to get the development environment up and running. You can just follow the steps below: 
<br/>
<br/>
![](https://github.com/gorselanaliz/raspberry_pi_rplidar_ros/blob/main/ros_installation.gif)
<br/>

In order to install ROS Noetic on your Raspberry Pi is not different from any PC. You can follow the steps in offical ROS documentation in here: https://wiki.ros.org/noetic/Installation/Ubuntu <br/><br/>
After installation you can check the version of your ROS just for understanding everything is OK
```
$ rosversion -d
```
Create a workspace and clone robopeak package in /src folder by following the steps below:
```
$ mkdir ~/lidar_ws
$ mkdir ~/lidar_ws/src

$ cd ~/lidar_ws/src
$ git clone https://github.com/robopeak/rplidar_ros.git
```

## Usage

Now, you're ready to start scanning

```
$ catkin_make rplidar_ros
$ source ~/lidar_ws/devel/setup.bash
$ roslaunch rplidar_ros view_rplidar.launch
```
<br/>

![](https://github.com/gorselanaliz/raspberry_pi_rplidar_ros/blob/main/result.gif)
<br/>

## Support

<a href="https://www.buymeacoffee.com/gorselanaliz" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>


<!-- CONTACT -->
## Contact

Project Link - [Udemy](https://www.udemy.com/course/yolov8-bilgisayarl-goru-ile-trafik-analizi-3-ozgun-proje)

Discord - [Discord](https://discord.gg/AEvZdFs5rF)

Instagram - [Instagram](https://www.instagram.com/gorselanaliz_/)


E-mail -  analizgorsel@gmail.com

<!-- LICENSE -->
## License
Distributed under the MIT License.

