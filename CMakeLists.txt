cmake_minimum_required(VERSION 3.15)

project(async_tcp_echo_server LANGUAGES CXX VERSION 1.0.0)

set(CMAKE_VERBOSE_MAKEFILE TRUE)

set(CMAKE_POSITION_INDEPENDENT_CODE TRUE)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

find_package(boost CONFIG REQUIRED)

file(GLOB SOURCE_FILES src/*.cpp)

add_executable(${PROJECT_NAME}
        ${SOURCE_FILES}
)

target_link_libraries(${PROJECT_NAME}
        boost::boost
)
