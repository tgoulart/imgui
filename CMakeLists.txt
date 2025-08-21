project(imgui)

add_library(imgui STATIC)

target_include_directories(imgui
  PUBLIC
    "${CMAKE_CURRENT_SOURCE_DIR}"
)

target_sources(imgui
  PUBLIC
    imconfig.h
    imgui_internal.h
    imgui.h
    imstb_rectpack.h
    imstb_textedit.h
    imstb_truetype.h
    misc/cpp/imgui_stdlib.h
  PRIVATE
    imgui_demo.cpp
    imgui_draw.cpp
    imgui_tables.cpp
    imgui_widgets.cpp
    imgui.cpp
    misc/cpp/imgui_stdlib.cpp
)
