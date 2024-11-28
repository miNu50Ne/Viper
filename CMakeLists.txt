cmake_minimum_required(VERSION 3.28)

project(VIPER)

set(CMAKE_C_STANDARD 17)
set(CMAKE_CXX_STANDARD 20)

file(GLOB_RECURSE SOURCE ${CMAKE_SOURCE_DIR}/viper_ws/*.cpp)

include_directories(${PROJECT_SOURCE_DIR}/app)
include_directories(${PROJECT_SOURCE_DIR}/component)

add_executable(${PROJECT_NAME} ${SOURCE})