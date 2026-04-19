# BeaconLoader

**BeaconLoader** is an optimized chunk loader system for Paper-based Minecraft servers, designed to keep loader areas active while reducing unnecessary server load.

> This repository contains **documentation only**.  
> Source code is private.

---

## Features

- TPS-aware loader tick engine
- Optimized villager processing
- Smart entity activation based on distance
- Zombie threat caching for villagers
- Configurable loader sizes
- Debug commands for inspection
- SQLite persistence for loader data

---

## Why BeaconLoader?

BeaconLoader was built to provide the benefits of chunk loaders without the heavy performance cost that many loader plugins introduce.

It focuses on:

- reducing villager AI overhead
- minimizing repeated chunk processing
- keeping farms functional without fully simulating everything like vanilla player-loaded areas
- giving server owners direct control through configuration

---

## Current supported systems

### Loader sizes
- 3x3
- 5x5
- 7x7

### Config-driven behavior
BeaconLoader currently reads and supports:

- loader radius
- loader item material
- loader display name
- tick interval
- TPS skip thresholds
- villager activation distances
- zombie threat distance
- villager movement settings
- villager panic settings
- villager inactive behavior
- villager low-TPS boost
- debug loader info limit

---

## Commands

| Command | Description |
|---|---|
| `/bloader give <player> <3x3\|5x5\|7x7>` | Give a loader item |
| `/bloader reload` | Reload plugin config |
| `/bloader debug` | Show debug status |
| `/bloader tps` | Show current TPS |
| `/bloader tickets` | Show loader ticket info |
| `/bloader randomticks [world]` | Show random tick speed |
| `/bloader loaderinfo` | Show active loader information |
| `/bloader entityinfo` | Show entity information inside loaders |
| `/bloader nms` | Show server/NMS environment info |

---

## Configuration

See:
- [config.md](config.md)
- [optimization.md](optimization.md)
- [commands.md](commands.md)
- [architecture.md](architecture.md)

---

## Performance notes

BeaconLoader is built around a few core optimization ideas:

- Villagers are processed in a controlled way
- Zombie threat checks are cached
- Loader ticking adapts when TPS drops
- Chunk lists are cached per loader
- Unnecessary repeated logic is avoided

This makes it suitable for servers that want chunk loading behavior without turning every loaded area into a full performance sink.

---

## Storage

BeaconLoader stores loader data in SQLite.

This allows loaders to persist across restarts without requiring flat-file tracking.

---

## Intended use

BeaconLoader is intended for:

- survival servers
- economy servers
- technical servers needing controlled loader behavior
- server owners who want chunk loading with tighter performance control

---

## Repository scope

This repository is for:

- documentation
- configuration reference
- command reference
- architecture notes
- optimization notes

This repository does **not** include:

- source code
- compiled plugin jar
- private implementation files

---

## Contact

For access, testing, or private development inquiries, contact the repository owner.

---

## Status

BeaconLoader is actively documented and refined.
