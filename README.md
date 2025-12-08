# App Graphics 3D

A comprehensive GPU programming project implementing various graphics APIs and rendering techniques using C++.

## Overview

This repository contains multiple implementations of 2D and 3D graphics rendering using different modern graphics APIs including DirectX 11/12, Vulkan, and OpenGL. The project demonstrates low-level GPU programming concepts and provides comparison examples across different graphics backends.

## Project Structure

### Graphics APIs Implementations

#### 3D Graphics Modules
- **graphics3d/** - Core 3D graphics abstractions
- **graphics3d_directx11/** - DirectX 11 implementation
- **graphics3d_directx12/** - DirectX 12 implementation
- **graphics3d_vulkan/** - Vulkan implementation
- **graphics3d_opengl/** - OpenGL implementation
- **graphics3d_khronos/** - Khronos group standards implementation

#### 2D Graphics Modules
- **draw2d_direct2d_directx12/** - Direct2D with DirectX 12 backend
- **aaa_draw2d_direct2d_directx12/** - Alternative Direct2D implementation
- **draw2d_directx12/** - DirectX 12 2D rendering
- **draw2d_vulkan/** - Vulkan 2D rendering
- **draw2d_opengl/** - OpenGL 2D rendering
- **draw2d_nanovg/** - NanoVG library integration
- **draw2d_vkvg/** - VKVG (Vulkan Vector Graphics) implementation

#### GPU Programming
- **gpu_directx12/** - DirectX 12 GPU compute
- **gpu_vulkan/** - Vulkan GPU compute

#### Text Rendering
- **write_text_direct2d_directx12/** - Text rendering with Direct2D
- **write_text_directx12/** - DirectX 12 text rendering

#### Demo Projects
- **hello3d/** - Basic 3D rendering introduction
- **cube/** - Rotating cube demo
- **impact3d/** - 3D physics/collision demo
- **continuum/** - Advanced rendering demo

#### Supporting Libraries
- **fuel2/** - Core utility library
- **fuel-memory-directx/** - DirectX memory management
- **fuel-memory-opengl/** - OpenGL memory management
- **fuel-window-directx/** - DirectX window management
- **fuel-window-opengl/** - OpenGL window management

## Features

- **Multi-API Support**: Compare implementations across DirectX, Vulkan, and OpenGL
- **2D and 3D Rendering**: Complete rendering pipelines for both 2D and 3D graphics
- **GPU Compute**: Direct GPU computation examples
- **Text Rendering**: Multiple approaches to text rendering
- **Memory Management**: Efficient GPU memory handling patterns
- **Window Management**: Cross-API window and context creation

## Prerequisites

### Windows
- Visual Studio 2019 or later
- Windows 10/11 SDK
- DirectX 12 SDK
- Vulkan SDK (for Vulkan implementations)

### General
- C++17 or later compiler
- CMake 3.15+ (if using CMake build system)
- OpenGL development libraries (for OpenGL implementations)

## Building

### Windows (Visual Studio)
```bash
# Navigate to specific module directory
cd graphics3d_directx12

# Open the solution file or use MSBuild
msbuild YourProject.sln /p:Configuration=Release
```

### CMake (if configured)
```bash
mkdir build
cd build
cmake ..
cmake --build . --config Release
```

## Usage

Each module can be built and run independently. Start with the demo projects:

1. **hello3d** - Learn basic 3D rendering setup
2. **cube** - Understand transformation matrices and rendering loops
3. **draw2d_*** - Explore 2D graphics capabilities
4. **gpu_*** - Learn GPU compute concepts

## Architecture

The project follows a modular architecture:
- **Core abstractions** in `graphics3d/` and `fuel2/`
- **API-specific implementations** in respective directories
- **Memory management** separated by API
- **Window/context creation** abstracted for portability

## Contributing

Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Follow existing code style
4. Test across multiple APIs when possible
5. Submit a pull request with clear description

## License

Please check with the repository owner for licensing information.

## Resources

- [DirectX Documentation](https://docs.microsoft.com/en-us/windows/win32/directx)
- [Vulkan Documentation](https://www.vulkan.org/)
- [OpenGL Documentation](https://www.opengl.org/documentation/)
- [Khronos Group Standards](https://www.khronos.org/)

## Contact

For questions or collaboration, please open an issue in this repository.