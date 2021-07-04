aux_source_directory(. CURRENT_DIR_SRCS)

# 指定生成 Business 链接库
add_library(filesystem ${CURRENT_DIR_SRCS})