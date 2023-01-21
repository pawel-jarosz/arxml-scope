cmake_minimum_required(VERSION 3.22)
project(arxml_scope)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wpedantic -Werror")

find_package(nlohmann_json 3.10.5 REQUIRED) # Parsing configuration file
find_package(Boost 1.30 COMPONENTS program_options REQUIRED) # Parsing command line arguments

add_executable(arxml_scope src/main.cpp)
