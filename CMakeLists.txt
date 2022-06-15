cmake_minimum_required(VERSION 3.18)

project(SSS2022 CXX)

add_subdirectory(src)

add_executable(main main.cpp src/vetrex.cpp src/vetrex.h)

target_link_libraries(main source-lib)

