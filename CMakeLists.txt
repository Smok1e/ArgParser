cmake_minimum_required(VERSION 3.21)

project(
    ArgParser
    VERSION 1.0.0
    DESCRIPTION "Simple argument parser for C++"
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_library(
    ArgParser
	src/ArgParser/ArgParser.cpp
)

target_include_directories(
    ArgParser PUBLIC include/
)
