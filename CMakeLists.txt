cmake_minimum_required(VERSION 3.10)

# 设置项目名称
project(flyerApp)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

# 指定 C 编译器
set(CMAKE_C_COMPILER "C:/Program Files/Microsoft Visual Studio/2022/Community/VC/Tools/MSVC/14.40.33807/bin/Hostx64/x64/cl.exe")
set(CMAKE_CXX_COMPILER "C:/Program Files/Microsoft Visual Studio/2022/Community/VC/Tools/MSVC/14.40.33807/bin/Hostx64/x64/cl.exe")
set(CMAKE_GENERATOR_TOOLSET "v143")


include_directories(${CMAKE_SOURCE_DIR}/inc/)

add_executable(flyerApp 
${CMAKE_SOURCE_DIR}/src/main.cpp
${CMAKE_SOURCE_DIR}/src/madgwickFilter.c
)

