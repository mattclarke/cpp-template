# Template C++ Project

Contains the libraries I like to use for most C++ project:
- [fmt](https://github.com/fmtlib/fmt)
- [spdlog](https://github.com/gabime/spdlog)
- [CLI11](https://github.com/CLIUtils/CLI11)
- [Catch2](https://github.com/catchorg/Catch2)

## Requirements

The only requirements to be manually installed on the system are `Python`, `pip`, `CMake` and a compiler which is at least C++14 compliant.

Dependencies are managed by [Conan](https://conan.io/).
Conan requires Python and pip installed on the system, then:
```
pip install conan
```

That should be it, Conan will be run automatically by CMake to download the dependencies.

## Build

As usual for a CMake project.
For example from the source directory do
```
mkdir build
cd build
cmake ..
cmake --build . -- -j8
```

or on Windows
```
mkdir build
cd build
cmake -G "Visual Studio 15 2017 Win64" ..
cmake --build . -- -maxcpucount:8
```

## Run

From the build directory
```
./bin/TemplateProject
```
