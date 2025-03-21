# Минимальная требуемая версия CMake
cmake_minimum_required(VERSION 3.10)

# Название проекта
project(MyProject CXX)

# Установка стандарта C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Добавление путей для заголовочных файлов библиотек
include_directories(
    ${CMAKE_SOURCE_DIR}/lib/multiprecision/include
    ${CMAKE_SOURCE_DIR}/lib/config/include
)

# Добавление основного исходного файла
add_executable(MyProject main.cpp)