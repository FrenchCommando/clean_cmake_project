cmake_minimum_required(VERSION 3.10)
project(tests)

enable_testing()
include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})
set(TOTO_TEST_FILES
        toto_tests.cpp
    )
add_executable(runTotoTests ${TOTO_TEST_FILES})
target_link_libraries(runTotoTests gtest gtest_main)
target_link_libraries(runTotoTests toto)
