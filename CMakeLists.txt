cmake_minimum_required(VERSION 3.23)
project(lp_solver)


set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake")

find_package(LPSOLVE REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main PUBLIC lpsolve)