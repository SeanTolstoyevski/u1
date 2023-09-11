# U1 - Example for VCPKG, CMake and Boost usage

U1 is a simple example of using Boost, CMake and VCPKG together.
It is a program that prints random uuid values ​​to the screen using boost's uuid sublibrary.

In order to compile this project, in your system;
* vcpkg
	- boost
* cmake
* msvc / gcc / llvm
must be installed.

## compilation steps

Some parameters in the steps below will vary depending on your system. After cloning the project, you need to run these steps by changing them according to your own system.

1. `cd u1`
2. `mkdir build`
3. `cd build`
4. `cmake -G "Visual Studio 17 2022"  -DCMAKE_TOOLCHAIN_FILE=d:\projs\vcpkg\scripts\buildsystems\vcpkg.cmake -DVCPKG_TARGET_TRIPLET=x64-windows-static ..`
5. `cmake --build .`

## Important Note

CMake is a very large and complex tool. Please note that this is a simple example.