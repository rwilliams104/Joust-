cmake_minimum_required(VERSION 3.31)

project(GroceryProject LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_PREFIX_PATH "/opt/homebrew/opt/qtbase")

find_package(Qt6 REQUIRED COMPONENTS Widgets)
find_package(Qt6 REQUIRED COMPONENTS Gui)

add_executable(Joust!
    main.cpp
)

target_link_libraries(Joust! PRIVATE Qt6::Widgets)
target_link_libraries(mytarget PRIVATE Qt6::Gui)
