# Copyright (c) 2024 DPTechnics bv
# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.20.0)

list(APPEND BOARD_ROOT ${CMAKE_CURRENT_SOURCE_DIR})

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(walter_golioth_demo)

target_sources(app PRIVATE src/main.c)
target_sources(app PRIVATE src/sensor_dht20.c)
