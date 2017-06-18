Vulkan tutorial examples and demos
===============
![vulkan_logo](Docs/assets/vulkanlogo.png)

The first part of the tutorial involves the use of vulkan to draw basic triangles every step. Each setp has its own subdirectory containing a complete copy of the tutorial for that setp

## Status

| Compiler         | Operating System                     | Architecture | Version String |
|------------------|--------------------------------------|--------------|----------------|
| Visual Studio 2017 | Windows 8.1 Build 16170            | x64          | MSVC 19.10.25017.0 |
| Visual Studio 2017 | Windows 8.1 Build 16170            | x86          | MSVC 19.10.25017.0 |

| Compiler         | Operating System                     | Architecture | Version String |
|------------------|--------------------------------------|--------------|----------------|
| Clang 3.8        | Android NDK r14b with Unified Header | arm64-v8a    | Android clang version 3.8.275480  (based on LLVM 3.8.275480) |
| Visual Studio 2015 | Windows 10 Build 16170             | x64          | MSVC 19.0.24215.1 |
| Visual Studio 2017 | Windows 10 Build 16170             | x64          | MSVC 19.10.25017.0 |
| GCC 6.2.0          | Linux Ubuntu 16.04.1 with kernel 4.8 | x64        | gcc version 6.2.0 20160901 |
| GCC 6.2.0          | Linux Tegra-Ubuntu 4.4.15          | aarch64      | gcc version 6.2.0 20160901 |

[![Build status](https://ci.appveyor.com/api/projects/status/994t283721pa8fo8/branch/master?svg=true)](https://ci.appveyor.com/project/heitaoflower/vulkan-tutorial/branch/master)

## <img src="Docs/assets/windowslogo.png" alt="" height="32px"> Windows
A Visual Studio solution file for compiling all example projects is included with the repository, examples will compile with VS2017 and WindowsSDK10.0.x.

The repository contains everything required to compile and build the example projects on Windows.

### Requirements
* VulkanSDK : 1.0.46.0
