# Third-Party Licenses

This firmware is built on open-source components, each under its own license.
The list below covers the major dependencies. Where a component is fetched at
build time (ESP-IDF, managed components), its full license text ships with that
component in your build tree.

| Component | Used for | License |
|-----------|----------|---------|
| **ESP-IDF** (Espressif) | RTOS, drivers, build system | Apache-2.0 |
| **LVGL** (v8.x) | Touchscreen UI toolkit | MIT |
| **Helix MP3 decoder** | MP3 audio decoding | RealNetworks RCSL / RPSL |
| **esp_codec_dev / codec_board** (Espressif) | ES8311 codec + I2S audio | Apache-2.0 |
| **Waveshare BSP / demo code** | Board bring-up reference (ST77916, CST816S) | See Waveshare repository |
| **esp-web-tools** | Browser firmware installer (`installer/`) | Apache-2.0 |

## Notes

- **MP3 patents** expired in 2017, so MP3 decoding carries no patent obligations.
- The **Helix decoder** is under RealNetworks' RCSL/RPSL terms — retain its
  copyright headers in any redistribution of source.
- **esp-web-tools** is loaded from a CDN by `installer/index.html`; it is not vendored
  into this repository.
- The **Waveshare demo** is referenced for hardware bring-up; consult the
  upstream repository (<https://github.com/waveshareteam/ESP32-S3-Touch-LCD-1.85C>)
  for its exact terms before redistributing any of its code.

## Not covered here

The **Bible audio recordings** are *not* software and are *not* part of this
repository. They are licensed separately by their rights holders and must be
obtained with proper permission. See [LICENSE](LICENSE) and the README.
