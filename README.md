# ⚡ BeaconLoader

> Advanced **chunk loader system** optimized for performance, TPS stability, and large-scale farms.

---

## 🚀 Features

* ⚡ **TPS-aware engine** → reduces workload automatically under lag
* 🧠 **Smart entity activation** (villagers & golems)
* 🧑‍🌾 **Villager AI optimization** (movement, panic, inactivity)
* 🧊 **Golem freeze system** (no lag when inactive)
* 📦 **Configurable loaders** (3x3, 5x5, 7x7...)
* 💾 **Persistent loaders** (SQLite storage)
* 🔄 **Live reload support** (`/bloader reload`)
* 🛠️ Built for **Paper / Spigot 1.21+**

---

## 📦 Installation

1. Download the plugin `.jar`
2. Place it in `/plugins`
3. Start your server
4. Configure `config.yml`
5. Done ✅

---

## 🎮 Commands

| Command                        | Description          |       |               |
| ------------------------------ | -------------------- | ----- | ------------- |
| `/bloader give <player> <3x3   | 5x5                  | 7x7>` | Give a loader |
| `/bloader reload`              | Reload config        |       |               |
| `/bloader tps`                 | Show TPS             |       |               |
| `/bloader tickets`             | Show chunk tickets   |       |               |
| `/bloader loaderinfo`          | Show loaders         |       |               |
| `/bloader entityinfo`          | Show entities        |       |               |
| `/bloader randomticks [world]` | Show randomTickSpeed |       |               |
| `/bloader debug`               | Debug status         |       |               |
| `/bloader nms`                 | Server info          |       |               |

---

## ⚙️ Configuration

See full configuration here:

👉 [`config.md`](./config.md)

---

## 🧠 How it works

BeaconLoader creates a **controlled simulation environment** for chunks:

* Only processes entities when needed
* Skips ticks when TPS drops
* Reduces AI load dynamically
* Keeps farms working without killing performance

---

## 📊 Performance

* Designed for **high-entity environments**
* Works perfectly with:

  * Villager farms 🧑‍🌾
  * Iron farms 🛡️
  * Crop systems 🌾
* Minimal impact on MSPT

---

## 🔧 Requirements

* Java 17+ (recommended 21)
* Paper / Spigot 1.21+

---

## 🧪 Compatibility

* ✔ Paper
* ✔ Spigot
* ✔ Purpur (recommended)

---

## 📌 Notes

* Config is **fully customizable**
* System is **adaptive to TPS**
* No need to restart server → just `/bloader reload`

---

## 👨‍💻 Author

Developed by **GianniHz**

---

## ⭐ Support

If you like this project:

👉 Give it a ⭐ on GitHub
👉 Use it on your server
👉 Improve it

---

## 🔥 Future Plans

* Crop simulation module 🌱
* Advanced NMS hooks ⚙️
* Per-loader limits 👥
* GUI system 🎛️

---

## 📜 License

Private project — documentation public only.
