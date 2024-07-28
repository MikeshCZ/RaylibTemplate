cmake_minimum_required(VERSION 3.14)
project(RaylibTemplate)

# Standard C++
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Add source files
set(SOURCES
    src/main.cpp
)

# Add header files
set(HEADERS

)

# Libraries
find_package(raylib)

# Create executable
add_executable(${PROJECT_NAME} ${SOURCES} ${HEADERS})

#Link raylib to main
target_link_libraries(${PROJECT_NAME} 
    raylib
)