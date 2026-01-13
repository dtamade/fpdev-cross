# FPDev Cross-Compilation Toolchains

Cross-compilation toolchains for FPC.

## Overview

This repository provides binutils and libraries needed for cross-compiling FPC programs to different target platforms.

## Available Targets

| Target | Description | Host Platforms |
|--------|-------------|----------------|
| win64  | Windows 64-bit | Linux x86_64 |
| arm-linux | ARM Linux (32-bit) | Linux x86_64 |
| aarch64-linux | ARM64 Linux | Linux x86_64 |

## Components

Each cross-compilation target includes:

- **binutils**: Cross-compiler toolchain (linker, assembler, etc.)
- **libraries**: Target platform system libraries

## Usage

```bash
# List available cross-compilation targets
fpdev cross list

# Install cross-compilation support for Windows
fpdev cross install win64

# Build for Windows from Linux
fpc -Twin64 myprogram.pas
```

## Mirrors

- **GitHub**: https://github.com/dtamade/fpdev-cross
- **Gitee**: https://gitee.com/dtamade/fpdev-cross (China)

## License

Various licenses depending on the toolchain components.
