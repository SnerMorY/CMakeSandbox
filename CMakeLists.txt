cmake_minimum_required(VERSION 4.2.1)

project(Sandbox)

add_executable(${PROJECT_NAME} main.cpp)
target_compile_options(${PROJECT_NAME} PUBLIC -Wall PUBLIC -Wextra PUBLIC -Wpedantic)

add_subdirectory(Greeting)
target_link_libraries(${PROJECT_NAME} greetlib)

add_subdirectory(new_feature)
target_link_libraries(${PROJECT_NAME} feature1)