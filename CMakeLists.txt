cmake_minimum_required(VERSION 3.15)
project(compressor)

find_package(ZLIB REQUIRED)

add_executable(${PROJECT_NAME} src/main.cc)
target_link_libraries(${PROJECT_NAME} ZLIB::ZLIB)
