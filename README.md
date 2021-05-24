##working
# px4-jetson-xavier-nx-setup
<br>
<br>

# 1. xavier nx setup
### ● xavier nx setup

<details><summary>[click to see]</summary>
  
  - used sdkmanager and jetpack4.5.1
</details>

<br>

### ● xavier nx setup - ROS1 melodic

<details><summary>[click to see]</summary>
  
  - Set up the ROS melodic and I followed [this site](https://junk-research-note.tistory.com/7)
  
  ~~~shell
$ git clone https://github.com/jetsonhacks/installROSXavier.git
$ cd installROSXavier
$ ./installROS.sh -p ros-melodic-desktop
$ rosdep init
$ rosdep update
$ ./setupCatkinWorkspace.sh
$ echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc

~~~
</details>

### ● xavier nx setup - mavros setup

<details><summary>[click to see]</summary>
  
  - Set up realsense sdk and ros packages and I followed [this site](https://github.com/zinuok/Xavier_NX), which is based on jetson hacks
  ~~~shell
$ sudo apt-get install ros-melodic-mavros ros-melodic-mavros-extras
$ cd && wget https://raw.githubusercontent.com/mavlink/mavros/master/mavros/scripts/install_geographiclib_datasets.sh
$ sudo bash ./install_geographiclib_datasets.sh   
~~~
</details>

<br>


https://github.com/IntelRealSense/realsense-ros
sudo apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade
reboot
