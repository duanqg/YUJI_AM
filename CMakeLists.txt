cmake_minimum_required(VERSION 2.8)

project(LSDC)

add_library(hello src/hello.cpp)
add_library(bye src/bye.cpp)

add_executable(main main.cpp)

target_link_libraries(hello bye)
target_link_libraries(main bye)
target_link_libraries(main hello)