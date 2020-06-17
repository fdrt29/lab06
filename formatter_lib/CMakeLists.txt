# Минимальная версия
cmake_minimum_required(VERSION 3.4)
project(formatter) # имя проекта

# Стандарт С++
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Создаем статическую библиотеку
add_library(formatter STATIC formatter.cpp)
# Указываем для цели папку с заголовочными фалами
target_include_directories(formatter PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
