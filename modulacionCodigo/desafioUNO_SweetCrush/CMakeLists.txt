cmake_minimum_required(VERSION 3.16)

project(desafioUNO_SweetCrush LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(desafioUNO_SweetCrush main.cpp
    abstraccionDeMemoria.h
    abstraccionDeMemoria.cpp
    logicaTablero.cpp
    logicaTablero.h)

include(GNUInstallDirs)
install(TARGETS desafioUNO_SweetCrush
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
