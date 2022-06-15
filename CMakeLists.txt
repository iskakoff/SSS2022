cmake_minimum_required(VERSION 3.18)

project(SSS2022 CXX)

add_subdirectory(src)
include_directories(src)

add_executable(main main.cpp)

target_link_libraries(main source-lib)

