install(FILES budgie-desktop-wayland.desktop DESTINATION ${CMAKE_INSTALL_DATADIR}/wayland-sessions)

if(KWIN_DEVELOPMENT)
install(FILES budgie-desktop-kwinwayland.desktop DESTINATION ${CMAKE_INSTALL_DATADIR}/wayland-sessions)
endif()
