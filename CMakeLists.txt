cmake_minimum_required(VERSION 3.7)
project(learn)

set(CMAKE_CXX_STANDARD 11)
find_package(OpenCV 3 REQUIRED)
include_directories(
        ${OpenCV_INCLUDE_DIRS}
)

set(SOURCE_FILES main.cpp)
add_executable(learn ${SOURCE_FILES})
target_link_libraries(learn ${OpenCV_LIBS})
