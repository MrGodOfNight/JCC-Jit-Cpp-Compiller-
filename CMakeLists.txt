cmake_minimum_required(VERSION 3.5)

set(PROJECT_NAME JCC)
project(${PROJECT_NAME})

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++20 -Wall")

file(GLOB 
CPP_SOURCES "src/*.cpp")

file(GLOB
  CPP_HEADERS "src/*.hpp", "src/*.h", "src/headers/*.hpp", "src/headers/*.h"
)

add_executable(${PROJECT_NAME} ${CPP_SOURCES} ${CPP_HEADERS})