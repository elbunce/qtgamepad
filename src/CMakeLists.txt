# Copyright (C) 2023 The Qt Company Ltd.
# SPDX-License-Identifier: BSD-3-Clause

# Generated from src.pro.

add_subdirectory(gamepad)
add_subdirectory(plugins)

# special case begin
if(TARGET Qt::Quick)
    add_subdirectory(imports)
endif()

