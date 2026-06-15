# Minimum CMake required
cmake_minimum_required(VERSION 3.22)

option(WITH_CSHARP "build csharp lib" OFF)

add_subdirectory(cmake)
if (WITH_CSHARP)
    add_subdirectory(csharp/src/Google.Protobuf)
endif()