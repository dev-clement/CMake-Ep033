add_executable(${EXECUTABLE_NAME} ./src/main.cpp)
target_link_libraries(${EXECUTABLE_NAME} PUBLIC ${LIBRARY_NAME})
target_include_directories(${EXECUTABLE_NAME} PUBLIC ./include/)
