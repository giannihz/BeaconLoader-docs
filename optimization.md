```md
# Optimization Notes

BeaconLoader is designed to reduce the cost of chunk loaders by controlling what gets processed and how often.

## Main optimizations

### 1. TPS-aware ticking
The loader engine can probabilistically skip work when server TPS is low.

### 2. Villager threat cache
Zombie-near checks are cached so villagers do not repeatedly perform expensive nearby scans every pass.

### 3. Batch-oriented villager processing
Villager logic can be distributed to reduce per-cycle spikes.

### 4. Cached loader chunk lists
Chunk lists are cached per loader instead of being rebuilt repeatedly.

### 5. Distance-based entity activation
Villager logic depends on configured player distance thresholds.

## Goal

Keep farms and loader logic usable without fully simulating every chunk at full cost all the time.
