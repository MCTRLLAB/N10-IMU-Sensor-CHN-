# N100-Sensor-for-ROS2-
This files are original files from Wheeltec company and ROS SDK has modifiled for ROS2 Foxy

For install process;

1. Create workspace and src folder
2. Change permission by 
	sudo chmod 666 -R /dev/ttyUSB0
3. Copy and extract zip file in src folder 
4. Go to "fdilink_ahrs" folder
5. Change type of "wheeltec_udev.sh" as follows;
	sudo chmod +x wheeltec_udev.sh
	sudo ./wheeltec_udev.sh
6. Back to workspace folder and 
	colcon build (If it cannot perform, please use sudo colcon build)
7. Source and add source command to ~/.bashrc file
8. Run by command
	ros2 launch fdilink_ahrs ahrs_driver.launch.py
