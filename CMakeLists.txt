cmake_minimum_required(VERSION 3.15)
project(AoC22)
# Set the C compiler
set(CMAKE_C_COMPILER "/usr/bin/clang-16")

# Set the C++ compiler
set(CMAKE_CXX_COMPILER "/usr/bin/clang++-16")
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED YES)
set(CMAKE_CXX_EXTENSIONS NO)

include(dependencies.cmake)

add_executable(day1.1 day1.1.cpp)
    # set_target_properties(${name} PROPERTIES LINK_FLAGS /STACK:10000000)
target_link_libraries(day1.1 PRIVATE Microsoft.GSL::GSL)
