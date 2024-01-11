cmake_minimum_required(VERSION 3.10)

project(AlgorithmVisualizer)

# add SDL include directory path
include_directories(${CMAKE_SOURCE_DIR}/include/sdl/include)

# add SDL lib directory path
link_directories(${CMAKE_SOURCE_DIR}/lib/sdl)


# create executable with source files
add_executable(AlgorithmVisualizer ${CMAKE_SOURCE_DIR}/src/main.cpp)

# link libs
target_link_libraries(AlgorithmVisualizer SDL2)


