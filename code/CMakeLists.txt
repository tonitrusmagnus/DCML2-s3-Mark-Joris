cmake_minimum_required(VERSION 3.26)
project(code C)

set(CMAKE_C_STANDARD 11)

#add_executable(code client.c)
add_executable(code server.c)
if(WIN32)
    target_link_libraries(code wsock32 ws2_32)
endif()