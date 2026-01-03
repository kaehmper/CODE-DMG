# CODE-DMG (Refactor Branch)

This branch begins the refactor to split the project into a pure emulator core library and a UI/host layer.

## Goal
- **CODE-DMG.Core**: .NET class library (no Raylib, no window loop).
- **CODE-DMG.App** (optional): standalone demo/host (Raylib).

## Status
- Only the initial scaffolding is added in this commit.
- Next commits will move code from `src/` into `src/CODE-DMG.Core/` and isolate Raylib usage.

## Notes
The original project is a C# Game Boy emulator with minimal Raylib usage and a simple CPU-driven loop (70224 T-cycles per frame).
