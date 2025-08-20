cmake_minimum_required(VERSION 3.30)
project(hash-library)
add_library(hash-library-md5)
add_library(hash-library::md5 ALIAS hash-library-md5)
target_sources(hash-library-md5 PRIVATE
	md5.cpp
)
target_sources(hash-library-md5 PUBLIC
	FILE_SET HEADERS
	BASE_DIRS ${CMAKE_CURRENT_LIST_DIR}
	FILES
		md5.h
)
install(
	TARGETS hash-library-md5
	FILE_SET HEADERS
)