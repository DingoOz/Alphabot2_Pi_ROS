# Alphabot2_Pi_ROS
Python based software to use ROS to control the Alphabot2 using Raspberry Pi 3 hardware

Alphabot2 is a robot platform developed and marketed by Waveshare.
Hardware kits are sold through Seeed Studios etc.

ROS is the Robot Operating System (www.ros.org)

Raspberry Pi is a single board computer sold by the Raspberry Pi foundation. As of January 2019 it is reported that there are 3.5M of these boards in the wild.

This software has been tested on the Ubuntu image published by Ubiquity Robotics for primary use with their Magni platform (https://www.ubiquityrobotics.com/)

## Assumptions
- You are familar with ROS
- You are building a robot using the Waveshare Alphabot2
- You are using a Raspberry Pi 3
- You are using the Ubuntu image (sd card) Ubuntu 16.04 with ROS Kinetic supplied by Ubiquity Robotics (https://downloads.ubiquityrobotics.com/)

## Links
Alphabot2
https://www.seeedstudio.com/AlphaBot2-robot-building-kit-for-Raspberry-Pi-3-Model-B-p-2937.html

Python example code and other documentation
https://www.waveshare.com/wiki/AlphaBot2-Pi

## Instructions (Incomplete)
*(Work in Progress)*

If you start with the Raspberry Pi image published by Ubiquity Robitics, you will need to alter the /boot/config.txt file. Without a change, the Alphabot2's GPIO will be treated as power and other buttons, causing random network resets and shutdown events when manipulating the GPIO.

- Step 1: Edit /boot/config.txt, commenting out dtoverlay=ubituity-led-buttons by adding a '#' in front on it.

- Step 2: Reboot



- TODO - If you want to use a Static IP and not the pifi based script for auto AP)

- TODO - Setup TightVNC


## TODO - Install
<WIP: Basically create a package in your ROS workspace called alphabot2, copy this code over and run catkin_make, restart roscore and then use rosrun to start the alphabot2 driver_node >

## Running the code
There are several ways to run this code.

The first is to use the built in roslaunch file which allows basic control using the any joystick or USB gamepad set up with Linux.






