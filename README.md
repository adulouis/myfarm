# Gazebo Terrain Tutorial

A ros package to load a texture farmland with bumps for simulation in Gazebo.

## Installation

1. Clone this repository into the `src` in your ROS1 workspace

        $ cd /path/to/ros/workspace/src/
        $ git clone git@github.com:adulouis/myfarm.git
        $ cd ../

2. Source the ROS system environment and source the Gazebo environment

        $ . /opt/ros/<ROS_DISTRO>/setup.bash
        $ . /usr/share/gazebo/setup.sh

3. Install dependencies and build the package

        $ rosdep install --from-paths src --ignore-src -r -y
        $ catkin_make

4. Source the workspace environment and launch the example

        $ . ./devel/setup.bash
        $ roslaunch myfarm farmland.launch

At this point, Gazebo should have launched and loaded the custom farmland. A common mistake is to forgot
to source the Gazebo environment in step 2.

## Images
Image of the Blender model
![Alt text](images/Screenshot(137).png)

Image of the model in Gazebo
![Alt text](images/Screenshot(141).png)
