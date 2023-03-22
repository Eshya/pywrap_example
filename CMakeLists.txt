cmake_minimum_required(VERSION 3.4...3.18)
project(cmake_example)

add_library(mickey STATIC src/mickey.cpp)
set_target_properties(mickey PROPERTIES POSITION_INDEPENDENT_CODE ON)


add_subdirectory(pybind11)
pybind11_add_module(cmake_example src/pywrap.cpp)
target_link_libraries(cmake_example PRIVATE mickey)
# EXAMPLE_VERSION_INFO is defined by setup.py and passed into the C++ code as a

