cmake_minimum_required(VERSION 3.28)

project(CppProjectTemplate
        VERSION 0.0.1
        LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD          17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS       OFF)

set(LIBRARY_NAME Library)
set(EXECUTABLE_NAME Executable)

option(COMPILE_EXECUTABLE "Whether to compile the executable")

add_subdirectory(my_lib/)
if (COMPILE_EXECUTABLE)
    add_subdirectory(app/)
else()
    message("Without exe. Compiling")
endif()
