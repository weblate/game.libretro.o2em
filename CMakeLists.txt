cmake_minimum_required(VERSION 3.1)
project(game.libretro.o2em)

list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR})

find_package(Kodi REQUIRED)
find_package(libretro-o2em REQUIRED)

set(O2EM_CUSTOM_BINARY ${O2EM_LIB}
    ${PROJECT_NAME}${CMAKE_SHARED_LIBRARY_SUFFIX})

build_addon(${PROJECT_NAME} O2EM "")