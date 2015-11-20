cmake_minimum_required(VERSION 3.3)
project(transcoder)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

include_directories(lib)
link_directories(lib)

set(SOURCE_FILES main.cpp)
add_executable(transcoder ${SOURCE_FILES})
target_link_libraries(transcoder mpg123)