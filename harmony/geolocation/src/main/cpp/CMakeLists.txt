cmake_minimum_required(VERSION 3.13)
set(CMAKE_VERBOSE_MAKEFILE on)

file(GLOB rnoh_geolocation_SRC CONFIGURE_DEPENDS *.cpp)
add_library(rnoh_geolocation SHARED ${rnoh_geolocation_SRC})
target_include_directories(rnoh_geolocation PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(rnoh_geolocation PUBLIC rnoh)

