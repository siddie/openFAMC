# CMAKE BUILD SCRIPT FOR LOADERS AND FAMC BY CWI
cmake_minimum_required (VERSION 2.6) 

SET(LIB_NAME BaseFAMC)

FILE (GLOB sources
		${CMAKE_CURRENT_SOURCE_DIR}/*.cpp
		${CMAKE_CURRENT_SOURCE_DIR}/*.c
		${CMAKE_CURRENT_SOURCE_DIR}/*.h
    )

add_library (${LIB_NAME} STATIC ${sources})