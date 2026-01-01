cmake_minimum_required(VERSION 3.16)
project("th-common-widget.qt" CXX)

find_package(Qt6 REQUIRED COMPONENTS Widgets)

FILE(GLOB_RECURSE SRC src/*.cc src/*.h)
add_library(th-common-widget-qt ${SRC})
target_link_libraries(th-common-widget-qt PUBLIC Qt6::Widgets)