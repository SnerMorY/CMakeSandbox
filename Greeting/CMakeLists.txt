add_library(greetlib greeting.cpp)

target_include_directories(greetlib
	PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)