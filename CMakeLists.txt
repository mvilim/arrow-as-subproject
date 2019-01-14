cmake_minimum_required(VERSION 3.0)

project(arrow-as-subproject VERSION 0.0.1)

set(ARROW_BUILD_STATIC ON)
set(ARROW_BUILD_SHARED ON)

set(ARROW_IPC ON)
set(ARROW_PLASMA ON)
set(ARROW_PARQUET ON)

add_subdirectory(arrow/cpp)
