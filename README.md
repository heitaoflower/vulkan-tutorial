Vulkan tutorial examples and demos
===============
![vulkan_logo](Docs/assets/vulkanlogo.png)

The first part of the tutorial involves the use of vulkan to draw basic triangles every step. Each setp has its own subdirectory containing a complete copy of the tutorial for that setp

## Building
The repository contains everything required to compile and build the examples on Windows.
## <img src="Docs/assets/windowslogo.png" alt="" height="32px"> Windows
A Visual Studio solution file for compiling all examples is included with the repository, examples will compile with VS2017 and WindowsSDK10.0.x.

If you're using a difference IDE or compiler you can use the provided CMakeLists.txt for use with [CMake](https://cmake.org/) to generate a build configuration for your toolchain.
### Requirements
* VulkanSDK : 1.0.46.0
