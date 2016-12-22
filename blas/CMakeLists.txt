cmake_minimum_required(VERSION 2.8.11)

project(liblinear)

# Find includes in corresponding build directories
set(CMAKE_INCLUDE_CURRENT_DIR ON)
# Instruct CMake to run moc automatically when needed.
set(CMAKE_AUTOMOC ON)

add_library(blas daxpy.c ddot.c dnrm2.c dscal.c)
