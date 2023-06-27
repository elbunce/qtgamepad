# Copyright (C) 2023 The Qt Company Ltd.
# SPDX-License-Identifier: BSD-3-Clause

# Generated from darwin.pro.

#####################################################################
## QDarwinGamepadBackendPlugin Plugin:
#####################################################################
qt_internal_find_apple_system_framework(FWFoundation Foundation) # special case
qt_internal_find_apple_system_framework(FWGameController GameController) # special case

qt_internal_add_plugin(QDarwinGamepadBackendPlugin
    OUTPUT_NAME darwingamepad
    PLUGIN_TYPE gamepads
    SOURCES
        main.cpp
        qdarwingamepadbackend.mm qdarwingamepadbackend_p.h
   LIBRARIES
        ${FWFoundation}
        ${FWGameController}
        Qt::Core
        Qt::Gamepad
        Qt::GamepadPrivate
        Qt::Gui
)

#### Keys ignored in scope 1:.:.:darwin.pro:<TRUE>:
# OTHER_FILES = "darwin.json"
# PLUGIN_EXTENDS = "gamepad"
