cmake_minimum_required(VERSION 3.24)
project(OpenCVDemo)

set(CMAKE_CXX_STANDARD 17)

set(OpenCV_DIR "D:/opencv/mingw_build/install")
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
add_executable(OpenCVDemo main.cpp / ORBextractor.cpp / ORBextractor.h)
target_link_libraries(OpenCVDemo ${OpenCV_LIBS})