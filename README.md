# Nelyx Engine

[![License: GPL v2](https://img.shields.io/badge/License-GPL%20v2-blue.svg)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
[![Base Engine](https://img.shields.io/badge/Base-Woof!%20(MBF21)-orange)](https://github.com/fabiangreffrath/woof)

Nelyx Engine is a work-in-progress Doom source port based on [Woof!](https://github.com/fabiangreffrath/woof), tailored specifically to power [Project Apocrypha](https://noverris.itch.io/projectapocrypha) and [Super Tux Doom](https://github.com/NelyxDev/supertuxdoom).

---

## Why Does the Nelyx Engine Exist?

On December 23, 1997, John Carmack released the source code of Linux Doom, providing one of the most optimized game engines of its era under a non-commercial license. On October 3, 1999, the code was re-released under the GNU General Public License v2.0, enabling developers worldwide to modify, build, and create commercial Doom engine forks. 

Over the years, the community built upon this foundation: TeamTNT released Boom in 1998, which led to MBF in 1999, followed by WinMBF, and eventually Woof!. 

Because Nelyx Engine inherits directly from Woof!, it is distributed under the GPL 2.0 license.

---

## Goals and Features

The primary objective of Nelyx Engine is to deliver a comfortable, plug-and-play, and flexible experience without requiring tedious setup or dealing with bad default configurations found in other ports.

### Target Platforms
| Platform | Status | Notes |
| :--- | :--- | :--- |
| **Windows** | Planned / Active | Primary development target |
| **Linux** | Planned / Active | Primary delelopment support, but I do need to install a distro on my computer |
| **macOS** | Planned | Native build support, but I need a Mac borrowed to make the build possible |
| **WASM (Web)** | In Consideration | Web-based gameplay support |
| **UWP (Xbox Dev Mode)** | Planned | Console testing environment |
| **Android** | In Consideration | Future release (Woof! Android porting requires extra work) |

---

## Powered Games

Nelyx Engine serves as the core framework for two distinct projects:

* **[Project Apocrypha](https://noverris.itch.io/projectapocrypha)** — Built for MBF21 standards, featuring extended mechanics and custom mapping features.
* **[Super Tux Doom](https://github.com/NelyxDev/supertuxdoom)** — Built with strict Vanilla Doom compatibility and classic 90s feeling.
* **Other Doom engine projects/games** that use MBF21 or lower (such as the original Doom, Chex Quest, Freedoom etc.)

---

## About the Author and Vision

Hi! I am Nelyx, a teen developer passionate about retro gaming. Since playing Doom for the first time in November 2025, I became captivated by how incredible id Tech engines are. 

Simply playing these classics wasn't enough — I wanted to give back to the community by creating boomer shooters that introduce new players to this awesome subgenre. This engine packages these experiences with zero friction: no DRM, no microtransactions, and no ads — just pure 90s arcade chaos.

> Special thanks to id Software, TeamTNT, the MBF project, and the Woof! development team for keeping the legacy alive.

---

## Building from Source

### Prerequisites
* C++ Compiler (MSVC, GCC, or Clang)
* CMake (v3.12 or higher)
* SDL2 development libraries

### Building Instructions
This still does not work.
```bash
# Clone the repository
git clone [https://github.com/nelyx.dev/nelyx-engine.git](https://github.com/NelyxDev/nelyx-engine.git)
cd nelyx-engine

# Create build directory and configure
mkdir build && cd build
cmake ..

# Compile
cmake --build . --config Release
