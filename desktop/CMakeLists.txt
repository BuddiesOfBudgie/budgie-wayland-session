if(KWIN_DEVELOPMENT)
install(FILES budgie-desktop-kwinwayland.desktop DESTINATION ${CMAKE_INSTALL_DATADIR}/wayland-sessions)
endif()

if(MAGPIE_DEVELOPMENT)
install(FILES budgie-desktop-magpiev1.desktop DESTINATION ${CMAKE_INSTALL_DATADIR}/wayland-sessions)
endif()

if(MIRIWAY_DEVELOPMENT)
add_subdirectory(miriway)
endif()
