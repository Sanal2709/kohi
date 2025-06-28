cmake_minimum_required(VERSION 3.16)

project(engine)

file(GLOB engine_SRC
     "src/*.h"
     "src/*.c"
)

add_library(${PROJECT_NAME} ${engine_SRC})
