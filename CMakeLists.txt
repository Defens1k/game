cmake_minimum_required(VERSION 3.1)

project(game)

include_directories(include)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED on)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")


add_executable(server src/server.cpp src/secure_queue.cpp src/connection.cpp include/connection.h include/message.h include/secure_queue.h)