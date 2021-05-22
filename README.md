# px4-jetson-xavier-nx-setup
<br>
<br>

# 1. xavier nx setup
### ● xavier nx sd card image file

<details><summary>[click to see]</summary>
  
  - Download the image file fomr nvidia [Jetson Download Center](https://developer.nvidia.com/embedded/downloads)   
     In my case, 4.5.1 was the latest one, so I downloaded this   
     
  - Write the image file to your sd card with [Rufus](https://rufus.ie/en/) or [Etcher](https://www.balena.io/etcher/), whatever with your way   
  ![image](https://user-images.githubusercontent.com/72853382/119228985-ab42ed80-bb50-11eb-98d7-162190234040.png)

</details>

<br>

### ● xavier nx setup - ROS1 melodic

<details><summary>[click to see]</summary>
  
  - Set up the ROS melodic and I followed [this site](https://www.stereolabs.com/blog/ros-and-nvidia-jetson-xavier-nx/)
  ~~~shell
  $ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
  $ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
  $ sudo apt update
  $ sudo apt install ros-melodic-desktop
  $ sudo apt install python-rosdep
  $ sudo rosdep init
  $ rosdep update
  $ echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc 
  $ source ~/.bashrc
  $ sudo apt-get install cmake python-catkin-pkg python-empy python-nose python-setuptools libgtest-dev python-rosinstall python-rosinstall-generator python-wstool build-essential git
  $ sudo apt-get install python-catkin-tools
  $ mkdir -p ~/catkin_ws/src 
  $ cd ~/catkin_ws/
  $ catkin build
  $ echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc 
  $ source ~/.bashrc
~~~
</details>

<br>

### ● xavier nx setup - Realsense T265, D435i setup

<details><summary>[click to see]</summary>
  
  - Set up realsense sdk and ros packages and I followed [this git](https://github.com/zinuok/Xavier_NX)
  ~~~shell
  $ cd
  $ git clone https://github.com/IntelRealSense/librealsense.git
  $ cd librealsense
  $ sudo apt-get update && sudo apt-get upgrade
  $ sudo apt-get install -y git libssl-dev libusb-1.0-0-dev pkg-config libgtk-3-dev


~~~
</details>

<br>
