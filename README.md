<p align="center">
  <img src="https://i.imgur.com/TOcoUFX.png" width="600">
</p>

<h1 align="center">⚡ BeaconLoader</h1>

<p align="center">
  <b>High-performance chunk loader system designed for modern Minecraft servers</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Minecraft-1.21+-brightgreen?style=for-the-badge">
  <img src="https://img.shields.io/badge/Platform-Paper%20%7C%20Spigot-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Performance-Optimized-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge">
</p>

---

## 🚀 Overview

**BeaconLoader** is a next-generation chunk loading system focused on:

* ⚡ Maximum performance
* 🧠 Intelligent entity control
* 📉 TPS stability under heavy load
* 🏗️ Large-scale farm support

Built specifically for servers that need **efficiency without breaking gameplay**.

---

## ✨ Key Features

### ⚡ Performance Engine

* TPS-aware execution system
* Dynamic workload reduction
* Smart tick skipping

### 🧠 Entity Optimization

* Villager AI control
* Golem freeze system
* Distance-based activation

### 🧑‍🌾 Farm Stability

* Fully compatible with:

  * Iron farms
  * Villager breeders
  * Crop systems

### 📦 Loader System

* Configurable sizes (3x3, 5x5, 7x7)
* Persistent storage (SQLite)
* Per-loader chunk management

---

## 🎮 Commands

```
/bloader give <player> <3x3|5x5|7x7>
/bloader reload
/bloader tps
/bloader tickets
/bloader loaderinfo
/bloader entityinfo
/bloader randomticks [world]
/bloader debug
/bloader nms
```

---

## ⚙️ Configuration

Full configuration documentation:

👉 [`config.md`](./config.md)

---

## 📊 Performance Impact

| Scenario        | Result            |
| --------------- | ----------------- |
| 1000+ villagers | Stable TPS        |
| Iron farms      | No break          |
| Heavy loaders   | Controlled        |
| Low TPS         | Auto optimization |

---

## 🧠 How It Works

BeaconLoader does **not** blindly load chunks.

Instead it:

* Controls entity simulation
* Skips unnecessary ticks
* Reduces AI load dynamically
* Keeps essential mechanics working

---

## 🔧 Requirements

* Java 17+ (Recommended: 21)
* Paper / Spigot 1.21+

---

## 🧪 Compatibility

* ✔ Paper
* ✔ Spigot
* ✔ Purpur

---

## 📌 Why BeaconLoader?

Unlike traditional chunk loaders:

❌ No lag spikes
❌ No uncontrolled entity ticking
❌ No TPS destruction

✔ Smart
✔ Adaptive
✔ Optimized

---

## 🔮 Roadmap

* 🌱 Crop simulation system
* ⚙️ NMS optimization layer
* 🎛️ GUI loader manager
* 👥 Per-player limits
* 📊 Advanced metrics

---

## 👨‍💻 Developer

**GianniHz**

---

## ⭐ Support

If you like this project:

* ⭐ Star the repository
* 🚀 Use it on your server
* 💡 Suggest improvements

---

## 📜 License

Private plugin — documentation public only.
