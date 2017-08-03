cmake_minimum_required (VERSION 2.8.11)
project(capnpc-c)

set(CMAKE_SUPPRESS_REGENERATION true)
include_directories(${CMAKE_SOURCE_DIR})
set(SOURCES capnpc-c.c c.capnp.c capn-malloc.c capn-stream.c capn.c schema.capnp.c str.c)

add_executable(capnpc-c ${SOURCES})