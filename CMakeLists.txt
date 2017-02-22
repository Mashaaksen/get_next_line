cmake_minimum_required(VERSION 3.6)
project(gnl)
set(CMAKE_C_FLAGS "-std=c99 -Wall -Wextra -Werror")

set(SOURCE_FILES get_next_file.c get_next_line.h)
add_executable(gnl ${SOURCE_FILES})
target_link_libraries(gnl ${CMAKE_SOURCE_DIR}/libft/libft.a)