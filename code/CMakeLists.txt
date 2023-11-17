cmake_minimum_required(VERSION 3.26)
project(code C)

set(CMAKE_C_STANDARD 11)
add_library(ws2_32)
add_executable(code
        client.c)