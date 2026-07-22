# NiceMCU Arduino Board Manager

[简体中文](./README.md)

Official Arduino board packages for NiceMCU BK-series chips.

## Quick Start

In Arduino IDE, open **File → Preferences** and add the following URL under **Additional Boards Manager URLs**:

```text
https://github.com/NiceMCU-01/arduino/releases/download/global/package_NICEMCU_BK_index.json
```

Then open **Tools → Board → Boards Manager**, search for `NICEMCU BK7238`, and install it.

> Use this stable URL. Arduino IDE will discover future releases automatically, so the configured URL does not need to change.

## Current Support

| Chip   | Board | Current Version | Host Environment |
| ------ | ----- | --------------- | ---------------- |
| BK7238 | WB3S  | 1.3.0           | Windows          |

The initial release provides a Windows toolchain only. Linux and macOS support will be added after complete toolchains have been verified.

## Installation

1. Install [Arduino IDE 2](https://www.arduino.cc/en/software).
2. Open **File → Preferences**.
3. Add the stable JSON URL above under **Additional Boards Manager URLs**.
4. Open **Tools → Board → Boards Manager**.
5. Search for `NICEMCU BK7238` and install the latest version.

## Using the Board

After installation:

1. Select `WB3S` under **Tools → Board**.
2. Select the connected serial port under **Tools → Port**.
3. Open or create an Arduino sketch, compile it, and upload it to the board.

Use the upload speed and serial connection method appropriate for the target hardware and project documentation.

## Updates

This repository distributes core packages, toolchains, and package indexes through GitHub Releases.

- `global`: the stable JSON index used by Arduino IDE.
- `support`: Windows compiler, packaging, and upload tools.
- `vX.Y.Z`: versioned board core packages and index snapshots.

Keep the same `global` URL configured in Arduino IDE. New installable versions will appear in Boards Manager after they are released.

## Migrating from the Legacy URL

The legacy Sparkleiot BK7238 Boards Manager URL can continue to be used by existing installations. New installations and future updates should use the NiceMCU stable JSON URL in this repository.

## Future Support

The initial release supports BK7238/WB3S. NiceMCU plans to add Arduino board support for additional BK-series chips as hardware and toolchains become ready.

## Support and Feedback

For installation, compilation, upload, or board compatibility issues, please open an [Issue](https://github.com/NiceMCU-01/arduino/issues) and include:

- Arduino IDE version
- Operating system version
- Board model, selected serial port, and upload speed
- Complete error message or serial log
- A minimal reproducible example, if available

For custom firmware or technical collaboration, please contact: [song@sparkleiot.com](mailto:song@sparkleiot.com).
