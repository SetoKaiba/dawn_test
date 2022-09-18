cmake_minimum_required(VERSION 3.23)
project(dawn_test)

set(CMAKE_CXX_STANDARD 23)

find_package(dawn CONFIG REQUIRED)

add_executable(dawn_test main.cpp)
target_link_libraries(dawn_test dawn::dawn dxguid.lib)
