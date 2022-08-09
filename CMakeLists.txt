cmake_minimum_required(VERSION 3.19)
project(libtxref_client)

set(CMAKE_CXX_STANDARD 11)

find_package(libtxref 1.0.1 REQUIRED)

add_executable(libtxref_client main.cpp)

target_link_libraries(libtxref_client txref::txref)
