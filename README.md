# Terrain Roamer

**Terrain Roamer** is my third-person 3D exploration platformer built with Godot and C#. Explore the landscape, jump between platforms and mushrooms, collect coins, and avoid falling off the world. The project combines gameplay systems with a modular architecture and automated testing.

## Gameplay

[View the gameplay recording](https://github.com/user-attachments/assets/2b9f55bc-e5c7-45b4-8e93-eb05945f1890)

## Features

- Third-person movement through a 3D environment.
- Jumping and mushroom-bounce mechanics.
- Coin collection and exploration objectives.
- Save/load functionality using save-file and serialization tooling.
- State-driven gameplay logic and dependency injection.
- Automated tests using GoDotTest and related testing libraries.
- Godot Forward+ rendering and Jolt physics configuration.

## Technology

- **Engine:** Godot .NET SDK 4.7.2
- **Language/runtime:** C# and .NET 8
- **Architecture and utilities:** Chickensoft LogicBlocks, AutoInject, Serialization, Collections, SaveFileBuilder, and related packages.
- **Testing:** GoDotTest, GodotTestDriver, Shouldly, and Moq.

## Getting started

### Requirements

- Godot .NET SDK 4.7.2
- .NET SDK 8
- Git LFS, for repository assets tracked with Git LFS

### Setup

1. Clone this repository.
2. Run `git lfs pull` to download LFS-managed files.
3. Open the project in Godot 4.7.2 with .NET support.
4. Allow Godot to import project resources, then run the project from the editor.

For C# development, open `GameDemo.sln` in a compatible IDE after the project has been opened once in Godot.

## Controls

- **W / A / S / D:** Move.
- **Space:** Jump or bounce. Hold Space while falling to bounce as soon as you land.

## Architecture and testing

The game uses state machines to separate gameplay logic from presentation, with Chickensoft packages supporting state management, dependency provisioning, serialization, and testability. The repository includes state diagrams under `docs/` and test-related dependencies in `GameDemo.csproj`.

Test execution has not been independently verified as part of this README update.

## Asset and dependency credits

This project uses third-party libraries and assets. The codebase references Chickensoft open-source packages for game architecture and testing. The existing project notes credit **GDQuest** for many 3D assets, **FreePD** for music, and CC0-licensed sound effects. Review the terms for each asset and dependency before redistributing them.

- [Chickensoft](https://chickensoft.games/)
- [GDQuest](https://www.gdquest.com/)
- [FreePD](https://freepd.com/)

## License note

The repository's current `LICENSE` file names Chickensoft Organization as the copyright holder. That file has not been changed in this documentation update; verify that it is the correct license for this repository and its contents before relying on it as the license for your own contributions.
