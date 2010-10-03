# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Kapec
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(venv NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

# VEnv modules
INSTALL (FILES src/stable.lua src/venv.lua DESTINATION ${INSTALL_LMOD})

# Install documentation
INSTALL(DIRECTORY doc/ DESTINATION ${INSTALL_DOC})
INSTALL(DIRECTORY tests/  DESTINATION ${INSTALL_TEST})
