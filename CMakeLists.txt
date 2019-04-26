cmake_minimum_required(VERSION 3.12)
project(hidapi)

set(CMAKE_C_STANDARD 99)
set(CMAKE_C_FLAGS "-Wall -Wextra -Wno-unused-parameter -Wno-cast-function-type -Wno-stringop-overflow -O2")

include_directories("hidapi")
add_library(hidapi "windows/hid.c")
