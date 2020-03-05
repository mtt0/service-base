cmake_minimum_required(VERSION 3.0)

project(ServiceBase)

set(SOURCES ServiceBase.cpp ServiceInstaller.cpp)

add_library(service_base STATIC ${SOURCES})

target_include_directories(service_base PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_compile_definitions(service_base PRIVATE UNICODE=1)
target_compile_features(service_base PRIVATE cxx_std_11)
