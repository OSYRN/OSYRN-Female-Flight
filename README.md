# OSYRN's Female Flight — source code

This is the matching source for **OSYRN's Female Flight 0.2.1**, including the optional FreeClimb Bridge.

**Looking to play?** Install the mod from [Nexus Mods](https://www.nexusmods.com/skyrimspecialedition/mods/196155). You do not need anything from this repository.

## Download the source

Open the [0.2.1 release](https://github.com/OSYRN/OSYRN-Female-Flight/releases/tag/v0.2.1) and download **OSYRN-Female-Flight-Complete-Source-0.2.1.zip**. It includes the modified code, required library sources, build instructions, configuration and license notices.

The complete source is in that named download. GitHub's automatically generated archives contain only this repository's information files.

## Build

Extract the complete source ZIP to a short folder path on Windows. Install Visual Studio 2022 C++ Build Tools, the Windows SDK, CMake 3.24 or newer, and Git. With CMake on your PATH, run:

```powershell
powershell -NoProfile -File .\build-release.ps1 -Target All -Jobs 4
```

See `SOURCE-BUILD.txt` inside the ZIP for outputs and tests. The build does not change your game or mod manager.

## Credits and licenses

Based on [Wingflight by ROSVER / RoVerehr](https://github.com/RoVerehr/Wingflight) and [FreeClimb by Epsilona / Eelta](https://github.com/Eelta/FreeClimb). OSYRN designed and tested the integration, with AI assistance for the implementation.

Wingflight code is GPL-3.0-or-later with its included exceptions. FreeClimb code is GPL-3.0-only, with its included library notices and exceptions. Keep the original license files and credits with the source. See `CREDITS.txt` for the full notices.

Animation and sound assets have separate permissions. They are not included in this source download or covered by its software licenses. Players should follow the requirements on Nexus.
