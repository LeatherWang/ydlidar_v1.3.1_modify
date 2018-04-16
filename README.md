YDLIDAR ROS PACKAGE V1.3.1
=====================================================================

ROS node and test application for YDLIDAR

Visit EAI Website for more details about YDLIDAR.

How to build YDLIDAR ros package
=====================================================================
    1) Clone this project to your catkin's workspace src folder
    2) Running catkin_make to build ydlidar_node and ydlidar_client
    3) Create the name "/dev/ydlidar" for YDLIDAR
    --$ roscd ydlidar/startup
    --$ sudo chmod 777 ./*
    --$ sudo sh initenv.sh

How to run YDLIDAR ros package
=====================================================================
There're two ways to run YDLIDAR ros package

1. Run YDLIDAR node and view in the rviz
------------------------------------------------------------
roslaunch ydlidar lidar_view.launch

You should see YDLIDAR's scan result in the rviz.

2. Run YDLIDAR node and view using test application
------------------------------------------------------------
roslaunch ydlidar lidar.launch

rosrun ydlidar ydlidar_client

You should see YDLIDAR's scan result in the console





雷达驱动升级日志
=====================================================================
2017-11-30 version:1.1.2

新增

   1.增加对现有所有EAI雷达支持

   2.增加Linux下非标准波特率的支持

   3.增加串口异常检测

改进

   1.修复雷达数据不稳定

   2.修复雷达没有数据

2017-12-16 version:1.2.0

   1.SDK统一平台

2018-04-4 version:1.3.1

   1.更新SDK版本到1.3.1

   2.添加采样率、扫描频率设置

   3.修改配置，统一YDLIDAR雷达ROS坐标系

   4.修复X4,S4雷达打不开现象

   5.增加G4 G4C F4Pro 掉电保护功能

   6.增加S4B低光功率设置

   7.修复关闭ROS节点等待时间长
   
   8.补偿每个激光点时间戳

