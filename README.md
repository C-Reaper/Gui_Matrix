# Project README

## Overview
The project is a C-based implementation of The Matrix visual effect, utilizing a windowing library to render the animation on a screen.

## Features
- Renders The Matrix visual effect.
- Supports cross-compilation for Linux, Windows, and Web assembly using Emscripten.
- Uses a simple windowing system for rendering and updating the matrix display.

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC)
- Make utility
- Standard development tools

## Build & Run
### Build Process
To build the project, navigate to the root directory of the project and run:

```sh
make -f Makefile.(os) all
```

Where `(os)` can be:
- `linux` for building on Linux.
- `windows` for building on Windows.
- `wine` for cross-compiling for Windows on Linux.
- `web` for compiling to Web assembly.

### Clean Rebuild
To clean and rebuild the project:

```sh
make -f Makefile.(os) clean
make -f Makefile.(os) all
```

### Execute
After building, you can execute the program using:

```sh
make -f Makefile.(os) exe
```

---

**Note:** The project assumes that necessary libraries are installed on your system for compiling and linking against. For example, on Linux, you might need `libX11` and other development packages installed.