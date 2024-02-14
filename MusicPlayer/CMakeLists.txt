cmake_minimum_required(VERSION 3.16)

project(MusicPlayer VERSION 0.1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt6 6.4 REQUIRED COMPONENTS Quick Multimedia REQUIRED)

qt_standard_project_setup()

qt_add_executable(appMusicPlayer
    main.cpp
    playercontroller.h playercontroller.cpp
)

qt_add_qml_module(appMusicPlayer
    URI MusicPlayer
    VERSION 1.0
    QML_FILES Main.qml
    QML_FILES AudioInfoBox.qml
    QML_FILES ImageButton.qml
    QML_FILES PlaylistPanel.qml

    RESOURCES
    assets/images/bach.jpg
    assets/images/van.jpg

    assets/icons/icon.ico
    assets/icons/next.png
    assets/icons/play.png
    assets/icons/pause.png
    assets/icons/previous.png
    assets/icons/add.png
    assets/icons/trash.png
    assets/icons/menu.png
    assets/icons/search.png
    assets/icons/close.png

    assets/audio/gstring.mp3
    assets/audio/symphone.mp3

    SOURCES playercontroller.h playercontroller.cpp
    SOURCES audioinfo.h audioinfo.cpp
    SOURCES audiosearchmodel.h audiosearchmodel.cpp
    QML_FILES SearchField.qml
    QML_FILES SearchPanel.qml
)

# Qt for iOS sets MACOSX_BUNDLE_GUI_IDENTIFIER automatically since Qt 6.1.
# If you are developing for iOS or macOS you should consider setting an
# explicit, fixed bundle identifier manually though.
set_target_properties(appMusicPlayer PROPERTIES
#    MACOSX_BUNDLE_GUI_IDENTIFIER com.example.appMusicPlayer
    MACOSX_BUNDLE_BUNDLE_VERSION ${PROJECT_VERSION}
    MACOSX_BUNDLE_SHORT_VERSION_STRING ${PROJECT_VERSION_MAJOR}.${PROJECT_VERSION_MINOR}
    MACOSX_BUNDLE TRUE
    WIN32_EXECUTABLE TRUE
)

target_link_libraries(appMusicPlayer
    PRIVATE Qt6::Quick Qt6::Multimedia
)

include(GNUInstallDirs)
install(TARGETS appMusicPlayer
    BUNDLE DESTINATION .
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
