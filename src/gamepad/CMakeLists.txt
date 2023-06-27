# Copyright (C) 2023 The Qt Company Ltd.
# SPDX-License-Identifier: BSD-3-Clause

# Generated from gamepad.pro.

#####################################################################
## Gamepad Module:
#####################################################################

qt_internal_add_module(Gamepad
    NO_GENERATE_METATYPES
    PLUGIN_TYPES gamepads
    SOURCES
        qgamepad.cpp qgamepad.h
        qgamepadbackend.cpp qgamepadbackend_p.h
        qgamepadbackendfactory.cpp qgamepadbackendfactory_p.h
        qgamepadbackendplugin.cpp qgamepadbackendplugin_p.h
        qgamepadkeynavigation.cpp qgamepadkeynavigation.h
        qgamepadmanager.cpp qgamepadmanager.h
        qtgamepadglobal.h
    DEFINES
        QT_BUILD_GAMEPAD_LIB
    LIBRARIES
        Qt::CorePrivate
    PUBLIC_LIBRARIES
        Qt::Core
        Qt::Gui
    PRIVATE_MODULE_INTERFACE
        Qt::CorePrivate
)

if(ANDROID)
    set_property(TARGET Gamepad APPEND PROPERTY QT_ANDROID_BUNDLED_JAR_DEPENDENCIES
        jar/QtAndroidGamepad.jar
    )
    set_property(TARGET Gamepad APPEND PROPERTY QT_ANDROID_LIB_DEPENDENCIES
        plugins/gamepads/libplugins_gamepads_androidgamepad.so
    )
endif()

#### Keys ignored in scope 1:.:.:gamepad.pro:<TRUE>:
# ANDROID_FEATURES = "android.hardware.gamepad"
qt_internal_add_docs(Gamepad
    doc/qtgamepad.qdocconf
)

