cmake_minimum_required(VERSION 2.8.11)

project(liblinear)

# Find includes in corresponding build directories
set(CMAKE_INCLUDE_CURRENT_DIR ON)
# Instruct CMake to run moc automatically when needed.
set(CMAKE_AUTOMOC ON)

add_library(linear linear.cpp tron.cpp)
target_link_libraries(linear blas)

add_subdirectory(blas)
