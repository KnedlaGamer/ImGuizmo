cmake_minimum_required(VERSION 3.30)

project(ImGuizmo)

set(CMAKE_CXX_STANDARD 23)

set(Source
        GraphEditor.cpp
        GraphEditor.h
        ImCurveEdit.cpp
        ImCurveEdit.h
        ImGradient.cpp
        ImGradient.h
        ImGuizmo.cpp
        ImGuizmo.h
        ImSequencer.cpp
        ImSequencer.h
)

add_library(${PROJECT_NAME} ${Source})
target_include_directories(${PROJECT_NAME} PUBLIC
        ../imgui
)