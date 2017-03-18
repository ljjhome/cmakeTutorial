CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(tutorial)

# The version number
set(tutorial_VERSION_MAJOR 1)
set(tutorial_VERSION_MINOR 0)

#configure a header file to pass some of the CMake settings
#to the source code

CONFIGURE_FILE(
	"${PROJECT_SOURCE_DIR}/tutorialConfig.h.in"
	"${PROJECT_BINARY_DIR}/tutorialConfig.h"
	)

# add the binary tree to the search path for include files
# so that we will find tutorialConfig.h

INCLUDE_DIRECTORIES("${PROJECT_BINARY_DIR}")
#add the excutable
ADD_EXECUTABLE(tutorial tutorial.cpp)
