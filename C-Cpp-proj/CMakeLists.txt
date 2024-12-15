cmake_minimum_required(VERSION 3.30) # Minimum CMake version
project(C-Cpp-Devops)                  # Name of your project

# Set the C++ standard
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CMAKE_EXPORT_COMPILE_COMMANDS True)

# Variable for executable name
set(EXECUTABLE_NAME c-cpp-proj)

# Add the executable target
add_executable(${EXECUTABLE_NAME} src/main.c)

# Include directories (optional)
target_include_directories(${EXECUTABLE_NAME} PRIVATE include)