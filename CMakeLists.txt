cmake_minimum_required(VERSION 3.20)
project(wxTest)

find_package(wxWidgets REQUIRED gl core base OPTIONAL_COMPONENTS net)
include(${wxWidgets_USE_FILE})

add_executable(wxTest src/main.cpp)
target_link_libraries(wxTest ${wxWidgets_LIBRARIES})