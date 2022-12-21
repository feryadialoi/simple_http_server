cmake_minimum_required(VERSION 3.24)
project(simple_http_server)

set(CMAKE_CXX_STANDARD 17)

link_libraries(ws2_32 wsock32)

add_executable(simple_http_server main.cpp http_tcpserver.cpp)
