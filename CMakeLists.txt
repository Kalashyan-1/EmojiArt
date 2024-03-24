cmake_minimum_required(VERSION 3.0)
project(EmojiArt)

find_package(OpenCV REQUIRED)

set(SOURCES 
	src/main.cpp
	src/check.cpp
	src/color.cpp
	src/size.cpp
	)

add_executable(${PROJECT_NAME} ${SOURCES})

target_link_libraries(${PROJECT_NAME} PRIVATE ${OpenCV_LIBS})
