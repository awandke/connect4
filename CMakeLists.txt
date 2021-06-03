cmake_minimum_required(VERSION 3.10)

# set the project name
project(connect4
        VERSION 1.0
        DESCRIPTION "connect 4 in c++ with ai"
        LANGUAGES CXX)

set_property(GLOBAL PROPERTY USE_FOLDERS ON)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED True)


# add source library
add_subdirectory(src)

# for main 
add_subdirectory(app)

# test directory
add_subdirectory(test)

# add sfml library
add_subdirectory(sfml)