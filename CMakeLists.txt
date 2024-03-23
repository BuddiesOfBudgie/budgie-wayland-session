cmake_minimum_required(VERSION 3.26)

# Ensure built-in policies from CMake are used
cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})

project(budgie-wayland-session
	DESCRIPTION "Scripts and data files for Budgie Wayland"
	VERSION 0.0.1
	LANGUAGES NONE
	)

# Set up GNU conventions and standard FHS paths
include(GNUInstallDirs)

option(ANACONDA_INITIAL_SETUP "Install configuration for Anaconda Initial Setup?" OFF)
option(SDDM "Install configuration for SDDM?" ON)
option(KWIN_DEVELOPMENT "Install desktop session file using KWin for development?" OFF)


add_subdirectory(desktop)

if(ANACONDA_INITIAL_SETUP)
add_subdirectory(initial-setup)
endif()

if(SDDM)
add_subdirectory(sddm)
endif()
