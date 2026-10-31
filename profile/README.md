<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../branding/pitlogger-wordmark-dark.png">
    <img alt="PitLogger" src="../branding/pitlogger-wordmark-light.png" width="420">
  </picture>
</p>

<p align="center"><b>Open telemetry and data logging for your car.</b></p>

PitLogger turns an ESP32-S3 and a cheap ELM327 OBD-II adapter into a small telemetry system:
live vehicle data in your browser, trouble codes, and recordings of every drive – no app store,
no cloud, no subscription.

**What it does**

- 🔌 Connects to ELM327 adapters via Bluetooth Low Energy
- 📊 Live dashboard over its own Wi-Fi – speed, RPM, temperatures, fuel trims and more, with
  session min / avg / max
- 🚗 Reads vehicle info (VIN) and trouble codes (stored, pending, permanent)
- 💾 Records drives as `.pitlog` files on a microSD card
- 🧩 Planned: GPS, add-on modules via ESP-NOW (custom displays, gear indicator, function buttons),
  over-the-air updates

**Open by design**

The `.pitlog` file format will be openly documented, and the converter (to CSV, GPX and more)
will be free – as a web app and as a standalone tool – so your data stays readable even if
this project ever stops.

> 🚧 PitLogger is in early development.

## Repositories

| | |
|---|---|
| [pitlog](https://github.com/PitLogger/pitlog) | Open `.pitlog` file format specification – free converter to CSV, GPX and more coming soon |
| [elm327-emulator](https://github.com/PitLogger/elm327-emulator) | ESP32 that behaves like an ELM327 adapter with a simulated car – develop and test OBD apps without a vehicle |

More will follow, including a module SDK for building your own add-ons.
