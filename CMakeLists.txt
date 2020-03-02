cmake_minimum_required (VERSION 3.0)

project(ServiceBase)

set(SOURCES ServiceBase.cpp ServiceInstaller.cpp)

add_library(service_base OBJECT ${SOURCES})

target_include_directories(service_base INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
