# Quarry Ridge

An early open-world prototype made with Unreal Engine 5.7: a soldier on a grassy ridge around an old
quarry pit. Walk and sprint around the rim, then jump into the off-road buggy and drive the dirt road
that loops around the quarry.

https://github.com/Jivraj-18/quarry-ridge/raw/main/media/quarry-ridge-gameplay.mp4

▶ [Watch the gameplay video](media/quarry-ridge-gameplay.mp4) (1 min: on foot, then driving)

> Work in progress: no goals or enemies yet. It's a world to walk and drive around in.

## Download and play

**[Download the latest release](https://github.com/Jivraj-18/quarry-ridge/releases/latest)**, Linux x86_64.

1. Download `QuarryRidge-v0.1.0-Linux.zip` (about 650 MB) and unzip it.
2. Run `./RealWorldGame.sh` inside the `QuarryRidge` folder.

Needs a GPU with Vulkan support and current drivers. On an NVIDIA RTX 2050 (4 GB) it runs at around
15–20 fps: the scene is heavy on grass and trees. On NVIDIA laptops with hybrid graphics, if the game
starts on the integrated GPU:

```sh
__NV_PRIME_RENDER_OFFLOAD=1 __VK_LAYER_NV_optimus=NVIDIA_only ./RealWorldGame.sh
```

A Windows version is planned.

## Controls

| On foot | |
|---|---|
| W A S D | Move |
| Shift | Sprint |
| Space | Jump |
| Mouse | Look (over-the-shoulder camera) |
| E | Get into the car (stand next to it) |

| Driving | |
|---|---|
| W | Accelerate |
| S | Brake / reverse |
| A D | Steer |
| Space | Handbrake |
| Mouse | Look around |
| E | Get out |

R restarts, Esc quits.

## What's in it

- A quarry landscape: a 23 m deep pit with rock benches, rolling meadows, pines, aspens and boulders
- Dense grass, ferns and wildflowers
- A dirt road looping around the pit, built as a Landscape Spline
- A soldier character with idle, walk, run and jump animations and an over-the-shoulder camera
- A drivable off-road buggy with Chaos vehicle physics, and E to get in and out

## Source code

The Unreal project and the scripts that build this level live in
[Jivraj-18/sky-meadow](https://github.com/Jivraj-18/sky-meadow) (level `Maps/Lvl_Quarry`, scripts
`tools/build_quarry.py`, `tools/build_quarry_road.py`, `tools/import_soldier.py`).

## Credits

- Made with Unreal Engine 5.7 (© Epic Games). Off-road buggy and vehicle setup from Epic's
  Vehicle template.
- Textures, rocks, trees and plants: [Poly Haven](https://polyhaven.com) (CC0).
- Soldier character and animations: [Mixamo](https://www.mixamo.com) (Adobe).
- Scene inspired by a frame from the "PUBG MOBILE - Erangel's New Imagination Plaza" trailer by
  PUBG MOBILE (CC BY 3.0, via Wikimedia Commons). Not affiliated with PUBG MOBILE, BGMI or Krafton.
