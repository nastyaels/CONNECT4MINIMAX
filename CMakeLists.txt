cmake_minimum_required(VERSION 3.22)
project(CONNECT4MINIMAX)

set(CMAKE_CXX_STANDARD 14)

add_executable(CONNECT4MINIMAX main.cpp)
find_package(OpenMP)
if(OpenMP_CXX_FOUND)
    target_link_libraries(CONNECT4MINIMAX PUBLIC OpenMP::OpenMP_CXX)
endif()