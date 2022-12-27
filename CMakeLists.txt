cmake_minimum_required(VERSION 3.8)

project(simple_zlib LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED on)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

include_directories("${PROJECT_SOURCE_DIR}/include")

find_package(ZLIB)
add_executable(GzipTest src/zlib_pipe.cpp)
target_link_libraries(GzipTest ZLIB::ZLIB)
