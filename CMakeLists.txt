cmake_minimum_required(VERSION 3.12)

project(stb)

file(GLOB stb_SOURCES
    ${PROJECT_SOURCE_DIR}/stb.cpp
)

add_library(stb STATIC ${stb_SOURCES})

target_include_directories(stb PUBLIC
    ${PROJECT_SOURCE_DIR}
)

