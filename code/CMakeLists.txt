cmake_minimum_required(VERSION 3.10)

project( lighttoy )

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

set(LIBTOY_INCLUDE ${PROJECT_SOURCE_DIR}/libtoy/inc)

add_subdirectory(libtoy)
add_subdirectory(toy)

add_subdirectory(unittests)



