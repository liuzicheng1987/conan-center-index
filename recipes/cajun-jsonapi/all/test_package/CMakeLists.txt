cmake_minimum_required(VERSION 3.15)
project(test_package CXX)

find_package(cajun-jsonapi REQUIRED)

add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} PRIVATE cajun-jsonapi::cajun-jsonapi)
set_target_properties(${PROJECT_NAME} PROPERTIES CXX_STANDARD 11)
