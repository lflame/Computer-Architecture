CMAKE_MINIMUM_REQUIRED(VERSION 3.5)
PROJECT(PA1)

add_compile_options(-g)
# add_compile_options(-O2)
# add_compile_options(-Wall -Wconversion -Wextra)

SET(PA1_INCLUDES
        include/bitset.hpp
        include/cache.hpp
        include/replacement_strategy.hpp
        include/trace.hpp
        include/utils.hpp
        include/brute_force_cache.hpp)

SET(PA1_SOURCES
        src/main.cpp
        src/trace.cpp)

SET(CMAKE_CXX_STANDARD 11)
SET(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)

ADD_EXECUTABLE(${PROJECT_NAME} ${PA1_SOURCES})
TARGET_INCLUDE_DIRECTORIES(${PROJECT_NAME} PRIVATE include)
