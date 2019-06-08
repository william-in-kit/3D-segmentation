cmake_minimum_required( VERSION 2.8 )
project( imageBasics )

# 添加c++ 11标准支持
set( CMAKE_CXX_FLAGS "-std=c++11" )

# 寻找OpenCV库
set(OpenCV_DIR "/home/william/opencv_root/build_opencv") 
find_package( OpenCV REQUIRED )
  
# 添加头文件
include_directories( ${OpenCV_INCLUDE_DIRS} )

add_executable( mask_rcnn mask_rcnn.cpp )
# 链接OpenCV库
target_link_libraries( mask_rcnn ${OpenCV_LIBS} )
