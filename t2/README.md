### 第二个练习
本练习给工程添加了多个目录，给每个子目录都可以添加一个CMakeLists.txt

(1) ADD_SUBDIRECTORY(src bin)将当前CMakeList下的src文件添加到当前的build文件中，并且运行src文件夹中的CMakeLists.txt

(2) SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin) 来修改输出的可执行文件的目录

(3) INSTALL指令用来执行安装，针对不同的待安装文件类型，来设置INSTALL。
