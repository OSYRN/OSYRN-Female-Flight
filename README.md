# OSYRN's Female Flight — source code

This is the matching source for **OSYRN's Female Flight 0.2.2**, including the optional FreeClimb Bridge.

**Looking to play?** Install the mod from [Nexus Mods](https://www.nexusmods.com/skyrimspecialedition/mods/196155). This GitHub download is for people who want to inspect, modify or build the code.

The controls were designed with **controllers in mind**, and keyboard controls are supported too. Jump, Sprint and Sneak follow Skyrim's mappings by default. A separate `WingflightControls.ini` lets you change the keyboard and controller flight actions independently.

## What changed in 0.2.2

- Sprint speed and the flight pose stay in step, including sideways and backward movement.
- Ordinary double-Jump takeoff enters low hover and follows hills and small bumps. Sprinting forward and double-tapping Jump gives a free running takeoff. Holding Sprint from low hover also lets you climb away from the ground.
- Holding and releasing Jump on the ground gives a smooth wing charge and an eight-times-normal-height jump. AWU's jump-height setting affects button-triggered airborne flaps; automatic wingbeats keep their ordinary strength.
- Weapons keep the female Mage hover legs and body height. Melee swings keep the torso and wings steadier; aiming, casting and blocking remain available. Armed flight no longer carries the usual on-foot sprint camera sway.
- Tap Sneak to toggle flying stealth. Hold it to descend with a gradual wing tuck. Releasing, pressing Jump or approaching the ground smoothly reopens the wings. Double-tap Sneak to leave flight.
- Improved low-hover stability on slopes, ground approach, wall handoffs and cleanup of sprint states that could stop stamina from recovering.
- Added smoother staff equipment transitions, subtler leg motion during manual wingbeats, and clearer controls settings. Staff animations retain their author's separate permission and credit; see the Nexus installation instructions.

These animation changes are for female player characters. Male and NPC animation sets are unchanged.

## Download the source

Open the [0.2.2 release](https://github.com/OSYRN/OSYRN-Female-Flight/releases/tag/v0.2.2) and download **OSYRN-Female-Flight-Complete-Source-0.2.2.zip**. It includes the modified code, required library sources, configuration, build instructions and license notices.

The complete source is in that named download. GitHub's automatically generated archives contain only this repository's information files.

## Build

Extract the complete source ZIP to a short folder path on Windows. Install Visual Studio 2022 C++ Build Tools, the Windows SDK, CMake 3.24 or newer, and Git. Open PowerShell in the extracted folder. With CMake on your PATH, run:

```powershell
cd .\Source
powershell -NoProfile -File .\build-release.ps1 -Target All -Jobs 4
```

See `SOURCE-BUILD.txt` inside the ZIP for outputs and checks. The build does not change your game or mod manager. The current gameplay testing used Steam Skyrim SE 1.6.1170; use the requirements on Nexus for the supported game and SKSE setup.

## Credits and licenses

Based on [Wingflight by ROSVER / RoVerehr](https://github.com/RoVerehr/Wingflight) and [FreeClimb by Epsilona / Eelta](https://github.com/Eelta/FreeClimb). OSYRN designed and tested the integration, with AI assistance for the implementation. Thanks to ROSVER for the detailed bug reports.

Wingflight code is GPL-3.0-or-later with its included exceptions. FreeClimb code is GPL-3.0-only, with its included library notices and exceptions. Keep the original license files and credits with the source. See `CREDITS.txt` for the full notices.

Animation and sound assets have separate permissions. They are not included in this source download or covered by its software licenses. Players should follow the requirements and credits on Nexus. Some wing-audio fallback warnings remain under investigation; this update does not claim to fix every audio combination.
