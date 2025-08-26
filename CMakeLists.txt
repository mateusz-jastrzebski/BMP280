cmake_minimum_required(VERSION 3.13)

add_library(BMP280
    src/BMP280.cpp
)

target_link_libraries(BMP280 PUBLIC pico_stdlib hardware_spi)

target_include_directories(BMP280 INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/src)
