add_library(feature1 feature1.cpp)

target_include_directories(feature1
    PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)