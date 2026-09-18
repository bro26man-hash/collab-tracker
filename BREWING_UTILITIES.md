# Reusable Brewing Utilities Found

## 1. Gravity & Recipe Calculators (Python)

### [rwilson4/homebrew-calc](https://github.com/rwilson4/homebrew-calc)
- **License:** Apache 2.0 | **Language:** Python | **Stars:** 1
- CLI tool: OG, FG, ABV, IBU, SRM, water chemistry, strike temp, mash efficiency
- pip-installable, well-structured package
- **Reuse potential:** HIGH — clean API, permissively licensed

### [chrisgilmerproj/brewday](https://github.com/chrisgilmerproj/brewday)
- **License:** MIT | **Language:** Python | **Stars:** 26
- Same calc surface + charts + data files for malt/hops/water/yeast
- Documented on ReadTheDocs
- **Reuse potential:** HIGH — reference implementation with data

## 2. Yeast Pitch Rate Tools

### [M0N0S0DIUM/Calculation-Station-2.0](https://github.com/M0N0S0DIUM/Calculation-Station-2.0)
- **Language:** TypeScript
- UI-based pitch rate calculator: cells needed, packages, viability, starter volume
- **Reuse potential:** MEDIUM — good frontend component

### [shanehead/brewski](https://github.com/shanehead/brewski)
- **License:** MIT | **Language:** Rust + TypeScript + Svelte
- Full pitch rate calculator + refractometer correction + gravity conversions
- Multi-platform desktop app (macOS, iOS, Android, Windows, Linux)
- **Reuse potential:** MEDIUM-HIGH — packaged tooling with modern UX

## 3. Fermentation Monitoring (Hardware + Software)

### [BrewBench/monitor](https://github.com/BrewBench/monitor)
- **Language:** JavaScript | **Stars:** 78 | **Forks:** 18
- Production-grade Arduino/ESP32 controller with web UI
- Supports: thermistors, DS18B20, PT100, DHT22, BMP280
- RIMS capable (heater/pump control)
- **Reuse potential:** HIGH — production firmware + UI reference

### [justinmklam/iot-sourdough-starter-monitor](https://github.com/justinmklam/iot-sourdough-starter-monitor)
- **License:** GPL-3.0 | **Language:** C++ | **Stars:** 94 | **Forks:** 9
- Complete IoT pipeline: ESP8266 → MQTT → Kinesis → S3 → Athena → web app
- Sensors: DHT22 (temp/humidity), VL6180X (distance), SSD1306 (display)
- 3D printed enclosure + custom PCB (KiCad)
- **Reuse potential:** HIGH — full cloud architecture pattern

### [BernhardSchlegel/BierBot-Bricks](https://github.com/BernhardSchlegel/BierBot-Bricks)
- **License:** GPL-3.0 | **Language:** C | **Stars:** 32 | **Forks:** 10
- ESP8266 firmware + cloud dashboard (bricks.bierbot.com)
- Gravity monitoring + temperature control
- Supports TH Origin (20A) and Raspberry Pi variant
- **Reuse potential:** HIGH — turnkey hardware product with API

### [DigitalHomebrew/BrewMonitor](https://github.com/DigitalHomebrew/BrewMonitor)
- **License:** GPL-2.0 | **Language:** C | **Stars:** 21
- AVR + IR airlock bubble counter
- Thingspeak + Pushover notifications
- Open-source PCB + 3D printed sensor
- **Reuse potential:** MEDIUM — airlock-based activity detection

## 4. Batch Journaling & Yeast Tracking

### [jsled/brew-journal](https://github.com/jsled/brew-journal)
- **Language:** Python (Django) | **Stars:** 11 | **Forks:** 3
- Tracks batches, yeast strains, gravity readings, hops
- Active IRC community (#homebrew)
- **Reuse potential:** MEDIUM — data model inspiration

## Utility Ranking (by reuse potential)

1. **homebrew-calc** — Clean Python, Apache 2.0, easiest to integrate
2. **brewday** — Same calculations + charts + data, well-documented
3. **BrewBench monitor** — Production-grade firmware + web UI
4. **iot-sourdough-starter-monitor** — Full IoT/cloud reference architecture
5. **BierBot-Bricks** — Turnkey hardware + cloud API
6. **brewski** — Modern multi-platform desktop app
7. **BrewMonitor** — Airlock-based fermentation activity detection
8. **brew-journal** — Data model for batch/yeast tracking
9. **Calculation-Station-2.0** — Frontend pitch-rate component
10. **FermWatch** — Device integration layer