cmake_minimum_required(VERSION 3.8)
project(vulkan_tutorial)

set(CMAKE_CXX_STANDARD 14)

# Config vulkan
if (WIN32)
    set(Vulkan_INCLUDE_DIRS "$ENV{VULKAN_SDK}/Include")
    if (CMAKE_SIZEOF_VOID_P EQUAL 8)
        set(VULKAN_LIBRARY "$ENV{VULKAN_SDK}/Lib/vulkan-1.lib")
        set(VULKAN_STATIC_LIBRARY "$ENV{VULKAN_SDK}/Lib/vkstatic.1.lib")
    else()
        set(VULKAN_LIBRARY "$ENV{VULKAN_SDK}/Lib32/vulkan-1.lib")
        set(VULKAN_STATIC_LIBRARY "$ENV{VULKAN_SDK}/Lib32/vkstatic.1.lib")
    endif()
elseif (APPLE)
    set(CMAKE_FIND_FRAMEWORK NEVER)
    find_library(VULKAN_LIBRARY MoltenVK)
    set(CMAKE_FIND_FRAMEWORK ONLY)
    find_library(VULKAN_STATIC_LIBRARY MoltenVK)
    find_path(VULKAN_INCLUDE_DIR NAMES vulkan/vulkan.h HINTS
            "${VULKAN_LIBRARY}/Headers")
else()
    find_path(VULKAN_INCLUDE_DIR NAMES vulkan/vulkan.h HINTS
            "$ENV{VULKAN_SDK}/include")
    find_library(VULKAN_LIBRARY NAMES vulkan HINTS
            "$ENV{VULKAN_SDK}/lib")
endif()
include_directories(${Vulkan_INCLUDE_DIRS})
list(APPEND LIBS ${VULKAN_LIBRARY})
message(STATUS "Vulkan Include dirs: ${Vulkan_INCLUDE_DIRS} and libs: ${VULKAN_LIBRARY}")

# Config glfw3
option(GLFW_BUILD_DOCS OFF)
option(GLFW_BUILD_EXAMPLES OFF)
option(GLFW_BUILD_TESTS OFF)
add_subdirectory(3rd_party/glfw)
include_directories(3rd_party/glfw/include)
list(APPEND LIBS glfw)

# Config glm
include_directories(3rd_party/glm)

# Config vulkan header
include_directories(3rd_party/vulkan-header)

# Config stb_image & tinyobjloader
include_directories(3rd_party/others)

# Demos
add_subdirectory(Tutorial01)
add_subdirectory(Tutorial02)
add_subdirectory(Tutorial03)
add_subdirectory(Tutorial04)
add_subdirectory(Tutorial05)
add_subdirectory(Tutorial06)
add_subdirectory(Tutorial07)
add_subdirectory(Tutorial08)
add_subdirectory(Tutorial09)
add_subdirectory(Tutorial10)
add_subdirectory(Tutorial11)
add_subdirectory(Tutorial12)
add_subdirectory(Tutorial13)
add_subdirectory(Tutorial14)
add_subdirectory(Tutorial15)
add_subdirectory(Tutorial16)
add_subdirectory(Tutorial17)
add_subdirectory(Tutorial18)
add_subdirectory(Tutorial19)
add_subdirectory(Tutorial20)
add_subdirectory(Tutorial21)
add_subdirectory(Tutorial22)
add_subdirectory(Tutorial23)
add_subdirectory(Tutorial24)
add_subdirectory(Tutorial25)
add_subdirectory(Tutorial26)
add_subdirectory(Tutorial27)
add_subdirectory(Tutorial28)
add_subdirectory(Tutorial29)
