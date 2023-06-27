# Generated from gamepads.pro.
# Copyright (C) 2022 The Qt Company Ltd.
# SPDX-License-Identifier: BSD-3-Clause

if(QT_FEATURE_sdl2)
    add_subdirectory(sdl2)
endif()
if(QT_FEATURE_evdev AND NOT ANDROID)
    add_subdirectory(evdev)
endif()
if(WIN32)
    add_subdirectory(xinput)
endif()
if(APPLE AND NOT WATCHOS)
    add_subdirectory(darwin)
endif()
if(ANDROID AND NOT android-embedded)
    add_subdirectory(android)
endif()
