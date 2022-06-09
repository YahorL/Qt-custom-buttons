cmake_minimum_required(VERSION 3.20)
project(Buttons)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_PREFIX_PATH "~/Qt/5.15.2/gcc_64/lib/cmake")

find_package(Qt5 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)


add_executable(Lab4
        main.cpp
        widget.cpp
        )
target_link_libraries(Lab4
        Qt::Core
        Qt::Gui
        Qt::Widgets
        )