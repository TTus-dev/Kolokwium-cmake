cmake_minimum_required(VERSION 3.10)
project(kol_zad4)
include_directories(include)
add_executable(kol_zad4 src/libtest.cpp)

add_library(kol_zad4_lib STATIC src/Student.cpp)
target_link_libraries(lib)

install(TARGETS kol_zad4_lib DESTINATION ./lib)
install(TARGETS kol_zad4 DESTINATION ./bin)
