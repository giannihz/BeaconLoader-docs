# ⚙️ BeaconLoader Configuration

## 📦 Loader Items

```yml
loaders:
  items:
    loader-3x3:
      radius: 1
      material: BEACON
      display-name: "&aLoader 3x3"

    loader-5x5:
      radius: 2
      material: BEACON
      display-name: "&aLoader 5x5"

    loader-7x7:
      radius: 3
      material: BEACON
      display-name: "&aLoader 7x7"
```

---

## ⚙️ Settings

```yml
settings:
  tick-interval: 20
  min-tps-safe: 10.0
  mid-tps-safe: 15.0
  skip-chance-low-tps: 0.50
  skip-chance-mid-tps: 0.20
```

Controls how the loader engine behaves based on server performance.

* `tick-interval` → How often loaders are processed (in ticks)
* `min-tps-safe` → TPS threshold for aggressive optimization
* `mid-tps-safe` → Medium TPS threshold
* `skip-chance-low-tps` → Chance to skip loader ticks under heavy lag
* `skip-chance-mid-tps` → Chance to skip loader ticks under moderate lag

---

## 🧠 Entity Activation

```yml
entity-activation:
  villager-distance: 48.0
  golem-distance: 32.0
  zombie-threat-distance: 10.0
```

Controls when entities are considered active.

* `villager-distance` → Distance from players to activate villagers
* `golem-distance` → Distance from players to activate golems
* `zombie-threat-distance` → Distance used for villager panic detection

---

## 🧑‍🌾 Villagers

```yml
villagers:
  enabled: true

  persistent: true
  remove-when-far-away: false

  active:
    move-chance: 0.03
    min-random-move: -0.10
    max-random-move: 0.10

  panic:
    enabled: true
    min-random-move: -0.35
    max-random-move: 0.35

  inactive:
    aware: true
    slowdown-chance: 0.01
    slowdown-multiplier: 0.20

  low-tps-boost:
    enabled: true
    trigger-below: 12.0
    chance: 0.02
    multiplier: 1.10
```

### Behavior Overview

**General**

* `enabled` → Enables villager processing
* `persistent` → Prevents villagers from despawning
* `remove-when-far-away` → Vanilla despawn behavior

**Active behavior**

* Random movement when players are nearby

**Panic behavior**

* Movement when zombies are detected

**Inactive behavior**

* Reduces movement when no players are nearby

**Low TPS boost**

* Small movement boost when server TPS is low

---

## 🐞 Debug

```yml
debug:
  enabled: false
  max-loaderinfo-lines: 10
```

Controls debug output.

* `enabled` → Enables debug mode
* `max-loaderinfo-lines` → Limits output size for `/bloader loaderinfo`

---

## 📝 Notes

* All systems are **TPS-aware**
* The plugin **automatically reduces workload** when the server is under stress
* Configuration changes can be applied using:

```
/bloader reload
```
