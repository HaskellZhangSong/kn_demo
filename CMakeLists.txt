cmake_minimum_required(VERSION 3.16)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON CACHE INTERNAL "") 

set(CMAKE_C_COMPILER "clang")
set(CMAKE_CXX_COMPILER "clang++")

add_executable(demo main.c)

target_include_directories(demo PRIVATE include)

target_link_directories(demo PRIVATE "lib")
target_link_libraries(demo native)


