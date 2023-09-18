project (HELLO_WORLD
        LANGUAGES C) # Используем язык C
cmake_minimum_required(VERSION 2.8.12) # Минимальная допустимая версия CMake
add_executable (helloWorld main.c) # Бинарный файл находится в build/helloWorld
add_compile_options(-Wall -Wextra -Wpedantic) # Опции компиляции для предупреждений
set_property(TARGET helloWorld PROPERTY C_STANDARD 99) # Используем стандарт C99
set(EXECUTABLE_OUTPUT_PATH ..)