# Copyright (c) 2024 Nordic Semiconductor ASA
# SPDX-License-Identifier: Apache-2.0
#
# This CMake file is picked by the Zephyr build system because it is defined
# as the module CMake entry point (see zephyr/module.yml).

if(CONFIG_ZIGBEE_R22)
  zephyr_include_directories(include)

  add_subdirectory(lib)
  add_subdirectory(subsys)
endif()
