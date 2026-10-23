cmake_minimum_required(VERSION 3.16)
project(cofmusi CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS ON)

add_executable(cofmusi src/main.cpp)

target_include_directories(cofmusi PRIVATE third_party)
target_link_libraries(cofmusi PRIVATE dl pthread m)

target_compile_options(cofmusi PRIVATE -Wall -Wextra)

