cmake_minimum_required(VERSION 3.10...3.21)

# This is a custom CMake file for the Dear ImGui library,
# for use in the Atlas project.
project(ImGui)

# ImGui source files
add_library(ImGui STATIC
    "imgui.cpp"
    "imgui_demo.cpp"
    "imgui_draw.cpp"
    "imgui_widgets.cpp"
    "imgui_tables.cpp"
)

# Include directories
target_include_directories(ImGui PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")