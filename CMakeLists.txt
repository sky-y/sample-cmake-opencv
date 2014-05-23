#SET(OpenCV_DIR "C:/opencv_qt4/install") 
SET(OpenCV_DIR "C:/opencv/opencv/build") # where OpenCVConfig.cmake exists

CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT( SampleCMakeOpenCV )
FIND_PACKAGE( OpenCV REQUIRED )
ADD_EXECUTABLE( MyProject main.cpp )
TARGET_LINK_LIBRARIES( MyProject ${OpenCV_LIBS})
#INCLUDE_DIRECTORIES("C:/opencv_qt4/install/include")
INCLUDE_DIRECTORIES("C:/opencv/opencv/build/include")
