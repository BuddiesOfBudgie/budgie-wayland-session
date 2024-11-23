configure_file(budgie-miriway-wrapper.in budgie-miriway-wrapper @ONLY)

install(FILES budgie-desktop-miriway.desktop DESTINATION ${CMAKE_INSTALL_DATADIR}/wayland-sessions)
install(FILES miriway-shell.config DESTINATION ${CMAKE_INSTALL_DATADIR}/budgie-wayland-session)

install(PROGRAMS ${CMAKE_CURRENT_BINARY_DIR}/budgie-miriway-wrapper DESTINATION ${CMAKE_INSTALL_LIBEXECDIR})
