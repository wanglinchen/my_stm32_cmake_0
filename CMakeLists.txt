# CMake 最低版本号要求
cmake_minimum_required (VERSION 3.0)

# 项目信息
project (application)
message(STATUS "Building project: ${PROJECT_NAME}")

# set the build type
if(NOT CMAKE_BUILD_TYPE) 
    set(CMAKE_BUILD_TYPE Debug)
endif(NOT CMAKE_BUILD_TYPE)

if(CMAKE_BUILD_TYPE MATCHES Debug)
  message(STATUS "Build type: Debug")
elseif(CMAKE_BUILD_TYPE MATCHES Release)
  message(STATUS "Build type: Release")
endif()



add_subdirectory(application)
add_subdirectory(business)
add_subdirectory(modular)
add_subdirectory(hardware)
add_subdirectory(rtos)
add_subdirectory(filesystem)







