# ros-robot-arm-package
install of ROS Melodic:

$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

$ curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

$ sudo apt update

$ sudo apt install ros-melodic-desktop-full

$ echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc

$ source ~/.bashrc

$ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential

$ sudo apt install python-rosdep

$ sudo rosdep init

$ rosdep update

Installing the package:

$ cd ~/catkin_ws/src

$ sudo apt install git
  
$ git clone https://github.com/smart-methods/arduino_robot_arm 
 
$ cd ~/catkin_ws
  
$ rosdep install --from-paths src --ignore-src -r -y
  
$ sudo apt-get install ros-melodic-moveit
  
$ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui
  
$ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher
  
$ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control

$ catkin_make

$ roslaunch robot_arm_pkg check_motors.launch
