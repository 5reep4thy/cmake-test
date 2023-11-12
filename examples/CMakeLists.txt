
project(cmake_test)
add_executable(main main.cpp)
# include_directories(${CMAKE_CURRENT_SOURCE_DIR}/../include)
target_include_directories(main PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/../include)
target_link_libraries(main PRIVATE hello_world)
