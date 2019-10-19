cmake_minimum_required(VERSION 2.8)
project(ImGui)

set(ImGui_SOURCES
    "imgui.cpp"
    "imgui_draw.cpp"
    "imgui_widgets.cpp"
    "imgui_demo.cpp"
    )

add_library(ImGui STATIC ${ImGui_SOURCES})
target_include_directories(ImGui INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}")