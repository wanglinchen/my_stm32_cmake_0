# 查找当前目录下的所有源文件,将名称保存到 CURRENT_DIR_SRCS 变量
aux_source_directory(. CURRENT_DIR_SRCS)

# 指定生成 Business 链接库
add_library(business ${CURRENT_DIR_SRCS})