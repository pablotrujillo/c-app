cmake_minimum_required(VERSION 3.10)

# Project name and version
project(c_app VERSION 1.0)

# Set the C standard
set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED True)

# Define a variable for the binary name
set(APP_NAME my_app) # Replace "my_app" with your desired default binary name

# Set the output directory for the binary
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin/)

# Add the executable
add_executable(${APP_NAME} src/main.c src/other_source.c)