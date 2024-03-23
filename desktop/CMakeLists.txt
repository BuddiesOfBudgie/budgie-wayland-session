install(FILES budgie-desktop-xwayland.desktop DESTINATION ${CMAKE_INSTALL_DATADIR}/wayland-sessions)

if(KWIN_DEVELOPMENT)
install(FILES budgie-desktop-kwinxwayland.desktop DESTINATION ${CMAKE_INSTALL_DATADIR}/wayland-sessions)
endif()
