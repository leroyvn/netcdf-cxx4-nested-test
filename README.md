# netcdf-cxx4 nested build test

## Requirements

- cmake
- miniconda3
- netCDF in line with netcdf-cxx4's requirements (4.6.0+); the conda default channel provides a libnetcdf package (v4.6.0 to v4.7.3 on 2020-02-21)

**Tested with cmake 3.16, libnetcdf 4.7.3.**

## How to build the project

- Navigate to the root of this project
- Configure the project:
  ```
  $ cmake . -B build -GNinja
  ```
- Build the project:
  ```
  $ cmake --build build
  ```
- Try and run the compiled application:
  ```
  $ ./build/src/main
  ```