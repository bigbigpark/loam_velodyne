Forked from https://github.com/laboshinl/loam_velodyne

<br/>

# loam_velodyne

Tested with ROS melodic on Ubuntu 18.04

<br/>

## How to build

```bash
$ cd ~/catkin_ws/src
$ git clone https://github.com/bigbigpark/loam_velodyne.git
$ cd ..
$ catkin build
```

<br/>

## How to run

* Run code below at two terminals respectively

```bash
$ roslaunch loam_velodyne loam_velodyne.launch
$ rosbag play nsh_indoor.bag
```

<br/>

## Troubleshooting

When an error of **multiscanRegistration** occurs, change things below at CMakeLists.txt.

Comment that line

~~~cmake
add_definitions(-march=native)
~~~

<br/>
