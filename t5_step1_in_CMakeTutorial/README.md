本练习来自于CMAKE官网的tutorial，step1包含知识点如下
(1)构建config文件，来给项目添加版本信息
(2)使用了config_file命令，指明xxConfig.h.in文件和xxConfig.h文件位置
(3)在CMakeLists.txt中用set命令设定version值
(4)在xxConfig.h.in文件中将version值与CMakeLists中设定值关联
(5)在main函数中使用该值
