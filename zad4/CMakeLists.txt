cmake_minimum_required(VERSION 3.10)
project(zad4)
include_directories(include)
add_executable(zad4 src/libtest.cpp)

add_library(zad4_lib STATIC src/Student.cpp)
target_link_libraries(zad4 zad4_lib)

install(TARGETS zad4_lib DESTINATION /lib)
install(TARGETS zad4 DESTINATION /bin)
