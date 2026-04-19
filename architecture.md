# Architecture

## Core classes

### BeaconLoader
Main plugin entrypoint.

### LoaderManager
Stores, loads, and removes loader records.

### LoaderAreaService
Handles chunk ticket loading, unloading, and cached chunk area lookup.

### LoaderTickEngine
Runs the main periodic loader processing loop.

### EntityController
Processes entity-related loader behavior.

### VillagerBrainController
Controls villager logic, awareness, and threat response.

### VillagerPathUpdateSystem
Applies configurable villager motion adjustments.

### BeaconDB
Stores loader data in SQLite.

## Runtime flow

1. Plugin starts
2. Database connects
3. Loaders are loaded from SQLite
4. Tick engine starts
5. Loader modules process entities each cycle
6. Config values control behavior
