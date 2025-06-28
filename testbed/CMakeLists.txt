cmake_minimum_required(VERSION 3.16)

project(testbed)

file(GLOB testbed_SRC
     "src/*.h"
     "src/*.c"
)

add_executable(${PROJECT_NAME} ${testbed_SRC})
target_include_directories(${PROJECT_NAME} PRIVATE "../engine/src")

target_link_libraries(${PROJECT_NAME} engine)
