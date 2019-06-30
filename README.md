Vulkan tutorial examples and demos <img src="https://img.shields.io/badge/license-MIT-blue.svg" title="license-mit" />
===============
![vulkan_logo](Docs/assets/vulkanlogo.png)

The first part of the tutorial involves the use of vulkan to draw basic triangles every step. Each setp has its own subdirectory containing a complete copy of the tutorial for that setp.

# Prerequisites
| | Windows | Linux | MacOS/iOS | Android |
|:---:|:---:|:---:|:---:|:---:|
|CI Status|[![Build status](https://ci.appveyor.com/api/projects/status/994t283721pa8fo8/branch/master?svg=true)](https://ci.appveyor.com/project/heitaoflower/vulkan-tutorial/branch/master)|TODO |TODO| TODO |
|Compiler| MSVC 14.0 | GCC 4.8+ | clang 3.6+ | NDK r12+ |
|OS Requirements| Win8.1 | Linux 3.14+ | MacOS Sierra | Adnroid 7.1+ |

# Generate project files

```bash
# UNIX Makefile
cmake ..

# Mac OSX
cmake -G "Xcode" ..

# Microsoft Windows
cmake -G "Visual Studio 14" ..
cmake -G "Visual Studio 14 Win64" ..
...
```

# Build Instructions
## <img src="Docs/assets/windowslogo.png" alt="" height="32px"> Windows

## Requirements
* VulkanSDK : 1.0.68.0

## <img src="Docs/assets/linuxlogo.jpg" alt="" height="32px"> Linux

## Requirements
* VulkanSDK : 1.0.68.0

## <img src="Docs/assets/maclogo.png" alt="" height="32px"> Mac

## Requirements
* VulkanSDK : 1.0.69.0
* MoltenVK : 0.19(Deprecated)
