cmake_minimum_required(VERSION 3.16)
project(imgui)

set(CMAKE_CXX_STANDARD 20)

set(CFLAGS -m64 -fvisibility=hidden)
set(CMAKE_POSITION_INDEPENDENT_CODE True)

set(IMGUI_SOURCE
        imconfig.h
        imgui.h
        imgui.cpp
        imgui_draw.cpp
        imgui_internal.h
        imgui_widgets.cpp
        imstb_rectpack.h
        imstb_textedit.h
        imstb_truetype.h
        imgui_demo.cpp
        )


add_library(imgui STATIC ${IMGUI_SOURCE})
