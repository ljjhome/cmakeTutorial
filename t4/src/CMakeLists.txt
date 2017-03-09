INCLUDE_DIRECTORIES("~/code/tmp/include")
LINK_DIRECTORIES("~/code/tmp/lib")
ADD_EXECUTABLE(jhello main.cpp)
TARGET_LINK_LIBRARIES(jhello hello)

