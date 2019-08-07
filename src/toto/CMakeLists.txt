cmake_minimum_required(VERSION 3.10)
project(toto)

set(CMAKE_CXX_STANDARD 17)

set(TOTO_SOURCE_FILES
        Toto.cpp Toto.h
    )

add_library(toto ${TOTO_SOURCE_FILES})
