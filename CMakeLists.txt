cmake_minimum_required(VERSION 3.0)
set(CMAKE_CXX_STANDARD 11)
include(cmake/HunterGate.cmake)
HunterGate(
    URL "https://github.com/hackallcode/hunter/archive/v0.19.170.1.tar.gz"
    SHA1 "64b918e50cf0dbc2d9d77a321a002c88ac186b54"
)
project(hello)
add_executable(hello ${CMAKE_CURRENT_SOURCE_DIR}/sources/hello.cpp)
install(TARGETS hello RUNTIME DESTINATION bin)
