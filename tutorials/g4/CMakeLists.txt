cmake_minimum_required(VERSION 3.16...3.27)
project(ehep-g4-basic)
find_package(Geant4 REQUIRED)
# Setup Geant4 include directories and compile definitions
include(${Geant4_USE_FILE})
add_executable(basic-g4 main.cpp)
target_link_libraries(basic-g4 ${Geant4_LIBRARIES})
