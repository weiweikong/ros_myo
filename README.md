ros_myo
=======

# Overview
This ROS package creates a ROS node which publishes raw data from the Thalmic Labs Myo Armband in the form of standard and custom ROS messages. These messages can be subscribed to and used in standard ROS architectures. 

Special thanks to Github user dzhu for creating the initial [myo-raw](https://github.com/dzhu/myo-raw) interface, which allowed for access to the raw data streaming from the Myo.

# Requirements
 - python >=2.6
 - pySerial
 - enum34

#Messages
There are three messages generated by the myo-rawNode.py node. These are:
  1. IMU: a standard IMU message with quaternion pose, accelerometer and gyro axes
  2. Arm: a custom arm Arm message that shows current arm and orientation on the arm
  3. EmgArray: a custom message that is comprised of floats which are the EMG readings from the eight sensors

#License
ros_myo is released with the MIT License. For full terms and conditions, see the [LICENSE](LICENSE) file
