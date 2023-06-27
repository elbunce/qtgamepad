# Copyright (C) 2023 The Qt Company Ltd.
# SPDX-License-Identifier: BSD-3-Clause

# Generated from evdev.pro.

#####################################################################
## QEvdevGamepadBackendPlugin Plugin:
#####################################################################

qt_internal_add_plugin(QEvdevGamepadBackendPlugin
    OUTPUT_NAME evdevgamepad
    PLUGIN_TYPE gamepads
    SOURCES
        main.cpp
        qevdevgamepadbackend.cpp qevdevgamepadbackend_p.h
    PUBLIC_LIBRARIES
        Qt::Core
        Qt::CorePrivate
        Qt::DeviceDiscoverySupportPrivatePrivate
        Qt::Gamepad
        Qt::GamepadPrivate
        Qt::Gui
)

#### Keys ignored in scope 1:.:.:evdev.pro:<TRUE>:
# OTHER_FILES = "evdev.json"
