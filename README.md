# U1 - Example for VCPKG, CMake and Boost usage

U1 is a simple example demonstrating the combined usage of Boost, CMake, and VCPKG. It is a program that displays random UUID values on the screen using Boost's UUID sublibrary.

To compile this project on your system, ensure the following dependencies are installed:

* vcpkg
	- boost
* cmake
* msvc / gcc / llvm

## compilation steps

Please note that certain parameters in the following steps may vary depending on your system configuration. After cloning the project, execute these steps, customizing them to match your own system:

1. `cd u1`
2. `mkdir build`
3. `cd build`
4. `cmake -G "Visual Studio 17 2022"  -DCMAKE_TOOLCHAIN_FILE=d:\projs\vcpkg\scripts\buildsystems\vcpkg.cmake -DVCPKG_TARGET_TRIPLET=x64-windows-static ..`
5. `cmake --build .`

## Important Note

CMake is a very large and complex tool. Please note that this is a simple example.
