cmake_minimum_required(VERSION 3.5)

project(QJsonStruct LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
#set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt5 COMPONENTS Core REQUIRED)


add_executable(QJsonStruct #STATIC
  QJsonStruct.hpp
  QJsonIO.hpp
  main.cpp
  TestIO.hpp
  TestOut.hpp
  macroexpansion.hpp
)

target_link_libraries(QJsonStruct Qt5::Core)
