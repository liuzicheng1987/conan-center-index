cmake_minimum_required(VERSION 3.15)
project(PackageTest C)

find_package(plutosvg CONFIG REQUIRED)

add_executable(test_package test_package.c)
target_link_libraries(test_package plutosvg::plutosvg)
