cmake_minimum_required(VERSION 2.8)
project(ImGui)

set(ImGui_sources
    "imgui.cpp"
    "imgui_draw.cpp"
    "imgui_widgets.cpp"
    "imgui_demo.cpp"
    )

add_library(ImGui STATIC ${ImGui_sources})
target_include_directories(ImGui PUBLIC "${PROJECT_SOURCE_DIR}")