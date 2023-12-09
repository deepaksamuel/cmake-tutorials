cmake_minimum_required(VERSION 3.15)
project(ehep-root-basic)
find_package(ROOT 6.28 CONFIG REQUIRED)

add_executable(basic-root main.cpp)
target_link_libraries(basic-root PUBLIC ROOT::Gui ROOT::Core)
