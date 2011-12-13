cmake_minimum_required(VERSION 2.8)
project(foo_pkg)
find_package(catkin REQUIRED)

add_executable(foo foo.cpp)

install(TARGETS foo
    DESTINATION share/foo_pkg/bin
    )

catkin_package(foo_pkg)
