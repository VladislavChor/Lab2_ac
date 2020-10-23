cmake_minimum_required(VERSION 2.8)	 # Проверка версии CMake.
										# Если версия установленой программы
										# старее указаной, произайдёт аварийный выход.

project(hello_world)			

add_library(
	hello 
	STATIC 
	hello.cpp
)	

add_executable(
	main 
	main.cpp
)	

target_link_libraries(main hello)		
