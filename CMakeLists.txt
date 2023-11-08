# CMakeList.txt : CMake project for AERSP_424_HW2, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project ("AERSP-424-HW-2-Final")

# Include SDL Directories
include_directories(${CMAKE_SOURCE_DIR}/SDL2-2.28.4/include)
link_directories(${CMAKE_SOURCE_DIR}/SDL2-2.28.4/lib/x64)


# Add source to this project's executable.
add_executable (AERSP-424-HW-2-Final "AERSP_424_HW2.cpp" "AERSP_424_HW2.h" "HW2_Visualizer.h" "HW2_Visualizer.cpp")

# Link SDL Libraries to Project
target_link_libraries(AERSP-424-HW-2-Final SDL2main SDL2)
