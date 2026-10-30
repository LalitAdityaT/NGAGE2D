# NGAGE2D

NGAGE2D is a C++20 2D game engine and a small bouncing-ball game built with it. Move the paddle to bounce the falling balls, build your score, and try to beat the saved high score.

## Features

- Scene-based engine with rendering, input, audio, timing, and resource managers
- Shader effects, including bloom, glitch, inverted-color, and monitor effects
- Paddle-and-ball gameplay with score, lives, music, and a persistent high score
- CMake-managed third-party dependencies

## Requirements

- CMake 3.28 or newer
- A C++20 compiler (for example, Visual Studio 2022 on Windows)
- An internet connection for CMake to download the project dependencies on the first configure

## Build and run

From the project directory:

```sh
cmake -S . -B Build
cmake --build Build --config Debug
```

Run the resulting `NGAGE2D` executable from the project directory so it can find the files in `Content/`. With the Visual Studio generator on Windows, the executable is typically `Build/Debug/NGAGE2D.exe`.

The VS Code build task is named **Build NGAGE2D (Debug)**.

## Controls

- **Left Arrow** / **Right Arrow**: move the paddle
- **Joystick X axis**: move the paddle

The high score is stored in `Content/Save.json`.

## Dependencies

CMake fetches these libraries during configuration:

- [SFML 3.0.2](https://github.com/SFML/SFML)
- [nlohmann/json 3.12.0](https://github.com/nlohmann/json)
- [spdlog 1.16.0](https://github.com/gabime/spdlog)
- [TGUI 1.11.0](https://github.com/texus/TGUI)
- [magic_enum 0.9.7](https://github.com/Neargye/magic_enum)

## License

This project is distributed under the MIT License. See [LICENSE](LICENSE).
