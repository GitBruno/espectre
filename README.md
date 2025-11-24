# 🛜 ESPectre Arduino Fork 👻

**Motion detection system based on Wi-Fi spectre analysis (CSI)**

---

## 🔧 Arduino Framework Fork

> **This is a fork of [ESPectre](https://github.com/francescopace/espectre) adapted for Arduino Framework integration.**
>
> **Key Differences from Upstream:**
> - ✅ **Arduino Framework Compatible**: Component library files work with Arduino/PlatformIO projects
> - ✅ **No Standalone Operation**: Designed to be embedded in larger Arduino applications (no `app_main()`)
> - ✅ **No External Dependencies Required**: No Home Assistant or MQTT broker needed when integrated
> - ✅ **Component Library**: Provides segmentation, CSI processing, and traffic generation as reusable modules
> - ✅ **Automatic Patching**: Build scripts handle compatibility fixes (`stdbool.h` includes, exclude main app)
>
> **Upstream Repository**: [francescopace/espectre](https://github.com/francescopace/espectre)  
> **Integration Example**: This repo allows ESPectre motion detection through a web interface without external MQTT infrastructure.
>
> **Note**: If you want standalone ESPectre with Home Assistant integration, use the [upstream repository](https://github.com/francescopace/espectre). This fork is for developers who want to embed ESPectre functionality into their own Arduino-based projects.

**📰 Featured Article**: Read the complete story behind ESPectre on Medium **[🇮🇹 Italian](https://medium.com/@francesco.pace/come-ho-trasformato-il-mio-wi-fi-in-un-sensore-di-movimento-40053fd83128?source=friends_link&sk=46d9cfa026790ae807ecc291ac5eac67&utm_source=github&utm_medium=readme&utm_campaign=espectre)**, **[🇬🇧 English](https://medium.com/@francesco.pace/how-i-turned-my-wi-fi-into-a-motion-sensor-61a631a9b4ec?sk=c7f79130d78b0545fce4a228a6a79af3&utm_source=github&utm_medium=readme&utm_campaign=espectre)**

**⚠️ Disclaimer**: This is an experimental project for educational and research purposes. The author assumes no responsibility for misuse or damage resulting from the use of this system. Use responsibly and in compliance with applicable laws.

---
