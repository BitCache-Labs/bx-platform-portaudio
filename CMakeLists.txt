# Portaudio lib
add_subdirectory (extern/portaudio)

add_library(bx-platform-portaudio STATIC 
    "src/bx/platform/audio_portaudio.cpp"
)
target_link_libraries(bx-platform-portaudio PRIVATE PortAudio)
target_include_directories (bx-platform-portaudio PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)