cmake_minimum_required(VERSION 4.2.1)

project(Sandbox)

add_executable(${PROJECT_NAME} main.cpp)
target_compile_options(${PROJECT_NAME} PRIVATE -Wall PRIVATE -Wextra PRIVATE -Wpedantic)

add_subdirectory(Greeting)

target_link_libraries(${PROJECT_NAME} greetlib)
