CMAKE_MINIMUM_REQUIRED(VERSION 3.0)
PROJECT(videostab)

FIND_PACKAGE(OpenCV REQUIRED)

ADD_EXECUTABLE(videostab
"${CMAKE_SOURCE_DIR}/main.cpp" 
)

TARGET_LINK_LIBRARIES(videostab ${OpenCV_LIBS})
