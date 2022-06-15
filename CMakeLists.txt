cmake_minimum_required(VERSION 3.18)

project(SSS2022 CXX)

find_package(MPI REQUIRED)

add_subdirectory(src)
include_directories(src)

add_subdirectory(test)
enable_testing()

add_executable(main main.cpp)
target_link_libraries(main source-lib MPI::MPI_CXX)

