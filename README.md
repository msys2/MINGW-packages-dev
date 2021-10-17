MINGW-packages-dev
==================

This repository contains package scripts for MinGW-w64 targets to build under MSYS2 for package maintainers.

## Documentation

See the [MSYS2 website](https://www.msys2.org/).

## Using packages

Download or clone the package folder with the scripts to your machine and build for yourself.

 Assuming you have a properly installed MSYS2 environment and build tools, you can build any package using the following command:
 ```
    cd ${package-name}
    MINGW_ARCH=mingw64 makepkg-mingw -sLf
 ```
 After that you can install the freshly built package(s) with the following command:
 ```
    pacman -U ${package-name}*.pkg.tar.zst
 ```
