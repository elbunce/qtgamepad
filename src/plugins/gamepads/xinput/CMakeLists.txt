# Copyright (C) 2023 The Qt Company Ltd.
# SPDX-License-Identifier: BSD-3-Clause

# Generated from xinput.pro.

#####################################################################
## QXInputGamepadBackendPlugin Plugin:
#####################################################################

qt_internal_add_plugin(QXInputGamepadBackendPlugin
    OUTPUT_NAME xinputgamepad
    PLUGIN_TYPE gamepads
    SOURCES
        main.cpp
        qxinputgamepadbackend.cpp qxinputgamepadbackend_p.h
    LIBRARIES
        Qt::Core
        Qt::Gamepad
        Qt::GamepadPrivate
        Qt::Gui
)

#### Keys ignored in scope 1:.:.:xinput.pro:<TRUE>:
# OTHER_FILES = "xinput.json"
