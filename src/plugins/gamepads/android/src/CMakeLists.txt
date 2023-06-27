# Copyright (C) 2023 The Qt Company Ltd.
# SPDX-License-Identifier: BSD-3-Clause

# Generated from src.pro.

#####################################################################
## QAndroidGamepadBackendPlugin Plugin:
#####################################################################

qt_internal_add_plugin(QAndroidGamepadBackendPlugin
    OUTPUT_NAME androidgamepad
    PLUGIN_TYPE gamepads
    SOURCES
        main.cpp
        qandroidgamepadbackend.cpp qandroidgamepadbackend_p.h
    LIBRARIES
        Qt::Core
        Qt::CorePrivate
        Qt::Gamepad
        Qt::GamepadPrivate
        Qt::Gui
)

#### Keys ignored in scope 1:.:.:src.pro:<TRUE>:
# DISTFILES = "android.json"
