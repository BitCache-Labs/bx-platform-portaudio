# Portaudio lib
#add_subdirectory (portaudio)

add_library(bx-platform-portaudio STATIC 
    "src/bx/platform/audio/audio_portaudio.cpp"
)
#target_link_libraries(bx-platform-portaudio PRIVATE glad)# imgui_opengl3)
target_include_directories (bx-platform-portaudio PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)