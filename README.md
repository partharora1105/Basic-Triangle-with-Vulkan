# Basic Triangle with Vulkan

This repository serves as a straightforward and minimalistic example illustrating the rendering of a triangle using the Vulkan graphics API. The primary aim of this project is to act as a foundational resource for developers seeking to grasp the fundamentals of Vulkan programming and establish a basic Vulkan application.
<p align="center">
  <img src="/github-images/1.png">
</p>

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Building the Project](#building-the-project)
- [Usage](#usage)
- [Resources](#resources)

## Getting Started

Please note that the steps outlined below have been tested on a Linux environment using Ubuntu.

### Prerequisites

Ensure all the necessary SDKs are installed by executing the following commands:

- Basic developer packages:

  ```bash
  sudo apt-get install build-essential
  ```

- Vulkan SDK:

  ```bash
  sudo apt install vulkan-tools
  ```

  Verify the installation by running:

  ```bash
  vkcube
  ```

- Vulkan Tools:

  ```bash
  sudo apt install vulkan-validationlayers spirv-tools
  ```

- GLFW Library:

  ```bash
  sudo apt install libglfw3-dev
  ```
- GLM Library:

  ```bash
  sudo apt install libglm-dev
  ```

- GLSLC:

  Install `glslc` from [GitHub Shaderc Releases](https://github.com/google/shaderc/blob/main/downloads.md). After extraction, copy `glslc` to your `bin`:

  ```bash
  cp '<path-to-extracted-directory>/install/bin/glslc' /usr/local/bin
  ```
### Building the Project

1. **Clone this repository:**

   ```bash
   git clone https://github.com/ypartharora1105/Basic-Triangle-with-Vulkan.git
   cd Basic-Triangle-with-Vulkan
   ```

   Use the provided makefile for easy compilation:

   ```bash
   make test
   ```

## Usage

Run the project with:

```bash
make test
```

To modify and compile shaders, adjust the contents of the `vertex` and `frag` files in the `shaders` directory, then compile them using:

```bash
<path-to-glslc>/glslc shader.frag -o frag.spv
<path-to-glslc>/glslc shader.vert -o vert.spv
```

## Resources

For official tutorials and in-depth learning, consider the following resources:

- [Vulkan API Documentation](https://www.khronos.org/registry/vulkan/)
- [Vulkan Online Tutorial](https://vulkan-tutorial.com/Drawing_a_triangle/Setup/Instance)
- [YouTube Vulkan Tutorial](https://www.youtube.com/watch?v=d2jkALhm9EE&list=PLRtjMdoYXLf4A8013lsFWHOgM9qdh0kjH) 
