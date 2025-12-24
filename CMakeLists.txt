
cmake_minimum_required(VERSION 3.16)
project(editor2d)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(SDL2 REQUIRED)

add_executable(editor2d
    src/main.cpp
)

target_include_directories(editor2d PRIVATE ${SDL2_INCLUDE_DIRS})
target_link_libraries(editor2d PRIVATE ${SDL2_LIBRARIES})

