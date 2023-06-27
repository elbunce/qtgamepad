# Copyright (C) 2023 The Qt Company Ltd.
# SPDX-License-Identifier: BSD-3-Clause

# Generated from gamepad.pro.

#####################################################################
## declarative_gamepad Plugin:
#####################################################################

qt_internal_add_qml_module(declarative_gamepad
    URI "QtGamepad"
    VERSION "1.${PROJECT_VERSION_MINOR}"
    CLASS_NAME QGamepadModule
    PLUGIN_TARGET gamepad
    DEPENDENCIES QtQuick
    NO_GENERATE_PLUGIN_SOURCE
    NO_GENERATE_QMLTYPES
    INSTALL_SOURCE_QMLTYPES "plugins.qmltypes"
    SOURCES
        qgamepadmouseitem.cpp qgamepadmouseitem.h
        qtgamepad.cpp
    PUBLIC_LIBRARIES
        Qt::Core
        Qt::Gamepad
        Qt::Gui
        Qt::Qml
        Qt::Quick
)

#### Keys ignored in scope 1:.:.:gamepad.pro:<TRUE>:
# CXX_MODULE = "gamepad"
# IMPORT_VERSION = "1.$$QT_MINOR_VERSION"
# OTHER_FILES = "qmldir"
# TARGETPATH = "QtGamepad"
