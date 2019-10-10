# ros_aruco
Simple ROS package for pose estimation using ArUco markers.
The package doesn't subscribe to topics such as Image and Camera Info compared to other existing ROS packages. 
This is done to avoid latency between the image publisher and the subscriber. 

How to use? 
1. Clone or download the package to your catkin workspace/src folder.
2. Set up your camera parameters such a camera matrix, distortion coefficients,
width and height of frame, fps in src/ros_aruco.cpp
3. Compile the package using catkin_make or catkin build.
4. Connect your USB camera to your PC.
5. Run roscore
6. Run the detection node via typing the following command on the terminal:
rosrun ros_aruco aruco_node
