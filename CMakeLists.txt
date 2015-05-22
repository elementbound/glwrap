cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project("glwrap" CXX)

SET(GLWRAP_SOURCES 	"window.cpp"
					"resizable_window.cpp"

					"mesh/basic_mesh.cpp"
					"mesh/separated_mesh.cpp"
					"meshutil.cpp"

					"texture.cpp"
					"texture_util.cpp"
					"fbo.cpp"

					"shader.cpp"
					"util.cpp")

add_library(glwrap ${GLWRAP_SOURCES})
add_definitions("-std=c++11")