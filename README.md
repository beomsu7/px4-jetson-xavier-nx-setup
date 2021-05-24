##working
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
  
  - Set up the ROS melodic and I followed [this site](https://junk-research-note.tistory.com/7)
$ git clone https://github.com/jetsonhacks/installROSXavier.git
$ cd installROSXavier
$ ./installROS.sh -p ros-melodic-desktop
$ rosdep init
$ rosdep update
$ ./setupCatkinWorkspace.sh
~~~
</details>

<br>

### ● xavier nx setup - Realsense T265, D435i setup

<details><summary>[click to see]</summary>
  
  - Set up realsense sdk and ros packages and I followed [this git](https://github.com/zinuok/Xavier_NX)
  ~~~shell



~~~
</details>

<br>
