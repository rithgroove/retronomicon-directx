cmake_minimum_required(VERSION 3.15)
project(retronomicon-directx VERSION 0.1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

if(NOT TARGET retronomicon)
    message(FATAL_ERROR "retronomicon-directx must be built from the workspace after retronomicon")
endif()

add_library(retronomicon-directx INTERFACE)
target_link_libraries(retronomicon-directx INTERFACE retronomicon)
target_compile_definitions(retronomicon-directx INTERFACE RETRONOMICON_GRAPHICS_BACKEND_DIRECTX=1)

message(STATUS "Building retronomicon-directx placeholder backend")
