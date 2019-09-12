cmake_minimum_required(VERSION 3.7)
project(openssl)

set(CMAKE_CXX_STANDARD 11)

file(GLOB_RECURSE SOURCES RELATIVE ${CMAKE_SOURCE_DIR} "*.c")
file(GLOB_RECURSE HEADERS RELATIVE ${CMAKE_SOURCE_DIR} "*.h")

include_directories("include/openssl")

add_executable(openssl ${SOURCES} ${HEADERS})