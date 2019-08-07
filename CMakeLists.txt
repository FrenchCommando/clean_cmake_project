cmake_minimum_required(VERSION 3.10)
project(CLEAN_CMAKE_PROJECT)

set(CMAKE_CXX_STANDARD 17)

include_directories(src)

add_subdirectory(libs/googletest)

add_subdirectory(src/toto)
add_subdirectory(tests/toto_test)
