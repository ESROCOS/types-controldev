# H2020 ESROCOS Project
# Company: DFKI
# Licence: GPLv2

# CMakeLists.txt has to be located in the project folder and cmake has to be
# executed from 'project/build' with 'cmake ../'.
cmake_minimum_required(VERSION 2.6)

include($ENV{ESROCOS_CMAKE})

project(types-controldev)

add_subdirectory(asn)
