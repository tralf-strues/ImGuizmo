add_library(ImGuizmo)

file(GLOB_RECURSE IMGUIZMO_INCLUDE *.hpp *.h)
file(GLOB_RECURSE IMGUIZMO_SOURCE *.cpp *.c)

target_include_directories(ImGuizmo
  PUBLIC
    ./
  )

target_sources(ImGuizmo
  PUBLIC
    ImGuizmo.h
  PRIVATE
    ImGuizmo.cpp
  )

target_link_libraries(ImGuizmo
  PUBLIC
    imgui
  )
