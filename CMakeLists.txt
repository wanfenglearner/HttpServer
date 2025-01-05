#cmake 最低版本
cmake_minimum_required(VERSION 3.00)
#项目名
project(HttpServer)
#C++11标准
set(CMAKE_CXX_STANDARD 11)
#debug模式
set(CMAKE_BUILD_TYPE Debug)

#设置输出路径
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_SOURCE_DIR}/bin)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR}/src SRC)

add_executable(httpserver ${SRC})












