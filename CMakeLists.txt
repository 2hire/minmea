cmake_minimum_required(VERSION 3.3)

project(minmea VERSION 0.3.1 LANGUAGES CXX)


add_library(minmea STATIC
    ${CMAKE_CURRENT_LIST_DIR}/minmea.cpp
    ${CMAKE_CURRENT_LIST_DIR}/minmea.h
)

target_compile_features(minmea PRIVATE cxx_std_20)
target_include_directories(minmea PUBLIC
	${CMAKE_CURRENT_LIST_DIR})

