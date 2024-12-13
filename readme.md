# 无人车SLAM及基于已知地图的自主导航

>说明：此仿真为BIT自动化学院zyp的无人平台技术仿真作业

# 1 运行环境 ros-noetic 需安装 move_base、gmapping 和 teb_local_planner

## move_base

```bash
sudo apt install ros-noetic-navigation
```

## gmapping

```bash
sudo apt-get install libsdl1.2-dev
sudo apt install libsdl-image1.2-dev


sudo apt-get install ros-noetic-gmapping
```

## teb_local_planner

```bash
sudo apt-get install ros-noetic-teb-local-planner
```

# 2 运行步骤

（1）命令行启动
```bash
roslaunch racecar_gazebo navi05.launch
```
（2）校准初始位置


启动后在 RVIZ 中 通过 2D Pose Estimate 将小车在 rviz 中移动至和 gazebo 中相近位置


（3）给定目标点


通过2D Nav Goal 给定目标点


# 3 说明

由于一些数据量过大，rosbag中只取了部分话题录制！