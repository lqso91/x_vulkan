cmake_minimum_required(VERSION 3.20)
project(x_vulkan)

set(CMAKE_CXX_STANDARD 17)

find_package(glfw3 REQUIRED)
find_package(Vulkan REQUIRED)
find_package(X11 REQUIRED)

#add_executable(x_vulkan main.cpp)
#add_executable(x_vulkan 00_base_code.cpp)
#add_executable(x_vulkan 01_instance_creation.cpp)
#add_executable(x_vulkan 02_validation_layers.cpp)
#add_executable(x_vulkan 03_physical_device_selection.cpp)
#add_executable(x_vulkan 04_logical_device.cpp)
#add_executable(x_vulkan 05_window_surface.cpp)
add_executable(x_vulkan 06_swap_chain_creation.cpp)

target_link_libraries(${PROJECT_NAME} glfw vulkan)