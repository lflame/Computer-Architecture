CMAKE_MINIMUM_REQUIRED(VERSION 3.5)
PROJECT(PA2)

add_compile_options(-g)
# add_compile_options(-O2)
# add_compile_options(-Wall -Wconversion -Wextra)

SET(PA2_SOURCES
        src/main.cpp
        src/test.cpp)

SET(CMAKE_CXX_STANDARD 11)
SET(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)

ADD_EXECUTABLE(${PROJECT_NAME} ${PA2_SOURCES})
TARGET_INCLUDE_DIRECTORIES(${PROJECT_NAME} PRIVATE include)
