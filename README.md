# 🛜 ESPectre Arduino Framework Fork 👻

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
>
> **Upstream Repository**: [francescopace/espectre](https://github.com/francescopace/espectre)  
> **Integration Example**: This repo allows ESPectre motion detection through a web interface without external MQTT infrastructure.
>
> **Note**: If you want standalone ESPectre with Home Assistant integration, use the [upstream repository](https://github.com/francescopace/espectre). This fork is for developers who want to embed ESPectre functionality into their own Arduino-based projects.

---

## 🔧 Integration with PlatformIO

Simply add to your `platformio.ini`:

```ini
[env:your_board]
platform = espressif32
board = esp32-s3-devkitc-1  ; or esp32-c6-devkitc-1
framework = arduino

; Add ESPectre library
lib_deps = 
    https://github.com/GitBruno/espectre.git#main
    ; ... your other libraries

; Force include stdbool.h for ESPectre compatibility (recommended)
build_flags = 
    -include stdbool.h
```

That's it! The library is **Arduino-ready by default**:
- ✅ All C files include `<stdbool.h>` (required by Arduino toolchain)
- ✅ No `espectre.c` with `app_main()` conflict (removed from repo)
- ✅ No test files (removed from repo)
- ✅ No build scripts needed (everything pre-configured)

**📰 Featured Article**: Read the complete story behind ESPectre on Medium **[🇮🇹 Italian](https://medium.com/@francesco.pace/come-ho-trasformato-il-mio-wi-fi-in-un-sensore-di-movimento-40053fd83128?source=friends_link&sk=46d9cfa026790ae807ecc291ac5eac67&utm_source=github&utm_medium=readme&utm_campaign=espectre)**, **[🇬🇧 English](https://medium.com/@francesco.pace/how-i-turned-my-wi-fi-into-a-motion-sensor-61a631a9b4ec?sk=c7f79130d78b0545fce4a228a6a79af3&utm_source=github&utm_medium=readme&utm_campaign=espectre)**

**⚠️ Disclaimer**: This is an experimental project for educational and research purposes. The author assumes no responsibility for misuse or damage resulting from the use of this system. Use responsibly and in compliance with applicable laws.

---
