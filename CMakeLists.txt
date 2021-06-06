cmake_minimum_required(VERSION 3.19)
project(<<TargetName>>)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(googletest)
include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})

add_executable(<<TargetName>> main.cpp)

add_executable(<<TargetName>>_Tests Tests.cpp)

target_link_libraries(<<TargetName>>_Tests gtest gtest_main)
