# only for cmake --version >= 3.5.1
cmake_minimum_required(VERSION 3.5.1)

# project name
project(kraken-engine-cmake)

# creates the variable EXEC and sets it to hello
set(EXEC kraken-engine)

# set the C++14 standard
set(CMAKE_CXX_STANDARD 14)

# I../includes
include_directories(include)

# puts all .cpp files inside src to the SOURCES variable
file(GLOB SOURCES src/*.cpp)

# compiles the files defined by SOURCES to generate the executable defined by EXEC
add_executable(${EXEC} ${SOURCES})