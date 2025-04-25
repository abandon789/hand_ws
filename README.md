相关依赖
mkdir -p hand_ws/src
cd hand_ws/src
sudo apt-get update
sudo apt-get install ros-noetic-aruco-ros
pip3 install transforms3d -i https://pypi.tuna.tsinghua.edu.cn/simple
cd .. && catkin_make
使用时需要source一下工作空间
source devel/setup.bash
roslaunch easy_handeye my.launch 
rqt_image_view
