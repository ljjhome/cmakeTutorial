SET(LIBHELLO_SRC hello.cpp)
ADD_LIBRARY(hello SHARED ${LIBHELLO_SRC})
ADD_LIBRARY(hello_static STATIC ${LIBHELLO_SRC})

SET_TARGET_PROPERTIES(hello_static PROPERTIES OUTPUT_NAME "hello")

INSTALL(TARGETS hello hello_static 
	LIBRARY DESTINATION "~/code/tmp/lib"
	ARCHIVE DESTINATION "~/code/tmp/lib"
	)

INSTALL(FILES hello.h DESTINATION "~/code/tmp/include")
