# Specify our lowest version number, make this a fatal error, since you don't
# since you don't want to deal with old versions EVER
cmake_minimum_required(VERSION 3.9.1 FATAL_ERROR) 

# Specify the project name, and the languages this project will support.
# CXX is C++
# C is C
# ASM is Assembly
# FORTRAN is fortran
# If this command isn't found in the top level CMakeLists.txt, CMake will add
# one with C and CXX enabled. The include command will not work for this.
project(HelloWorld CXX)

# If you have any global variables your whole project is going to need,
# set them before you add sub directories

# add_subdirectory can be thought of like a function call, except the function
# is another CMakeLists.txt, it even adds a scope, just like adding a function.
add_subdirectory(src)
