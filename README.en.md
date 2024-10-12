[English](README.en.md) | [日本語](README.md)

# jnmouse_description

ROS package with URDF description macro for [Jetson Nano Mouse](https://rt-net.jp/products/jetson_nano_mouse/)

![](https://rt-net.github.io/images/jetson-nano-mouse/jnmouse_rviz.png)

## Requirements

- ROS
  - [Humble Hawksbill](https://docs.ros.org/en/foxy/Releases/Release-Humble-Hawksbill.html)

## Installation

```sh
# jnmouse_descriptionをダウンロードして依存パッケージをインストールします
cd ~/colcon_ws/src
git clone https://github.com/rt-net/jnmouse_description
rosdep install -r -y -i --from-paths .

# パッケージをビルドします
cd ~/colcon_ws
colcon build
source install/setup.bash
```

## How to Use

Display the robot model of Jetson Nano Mouse on RViz with the following comand.

```sh
ros2 launch jnmouse_description display.launch.py
```

## LICENSE

(C) 2020 RT Corporation \<support@rt-net.jp\>

This repository is licensed under the Apache License, Version 2.0, see [LICENSE](./LICENSE).  
Unless attributed otherwise, everything in this repository is under the Apache License, Version 2.0.


### Acknowledgements

Special thanks to https://gbiggs.github.io/rosjp_urdf_tutorial_text/index.html