aux_source_directory(. CURRENT_DIR_SRCS)

add_executable(${PROJECT_NAME}.elf ${CURRENT_DIR_SRCS})

target_link_libraries(${PROJECT_NAME}.elf business modular hardware rtos filesystem)

target_include_directories(${PROJECT_NAME}.elf PRIVATE 
${PROJECT_SOURCE_DIR}/application
${PROJECT_SOURCE_DIR}/business
${PROJECT_SOURCE_DIR}/rtos
${PROJECT_SOURCE_DIR}/filesystem
)