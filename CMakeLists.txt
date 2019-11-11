project(libimgui)

set( IMGUI_SOURCES
  imgui_widgets.cpp
  imgui.cpp
  imgui_draw.cpp
  imgui_demo.cpp
  misc/cpp/imgui_stdlib.cpp
  misc/fonts/binary_to_compressed_c.cpp
)

set( IMGUI_HEADERS
  imconfig.h
  imgui_internal.h
  imgui.h
  imstb_rectpack.h
  imstb_textedit.h
  imstb_truetype.h
  misc/cpp/imgui_stdlib.h
)

add_library(imgui SHARED ${IMGUI_SOURCES} ${IMGUI_HEADERS})

include_directories(${PROJECT_SOURCE_DIR})