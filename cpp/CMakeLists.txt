cmake_minimum_required(VERSION 3.10)
project(kf_code)

add_subdirectory(thirdparty/pybind11)
include_directories(thirdparty/eigen)

pybind11_add_module(kf_cpp wrappers.cpp kf.h)