cmake_minimum_required(VERSION 3.24)

project(sample_lib)

include(GNUInstallDirs)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR}/${CMAKE_INSTALL_LIBDIR})

add_library(sample_lib source/src.cpp)
target_include_directories(sample_lib PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")