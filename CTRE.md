# Phoenix 2026 Beta 1

This is the 2026 beta 1 release of Phoenix software compatible with the 2026 FRC beta.

> [!IMPORTANT]  
>  CANivore functionality on roboRIO 2026.1.0 requires manual installation of the CANivore driver. See [CANivore Driver Installation](#canivore-driver-installation). This will be resolved in the next NI release.

> [!IMPORTANT]  
> 26.0.0-beta-1 requires 26.0.0 firmware

Please see our yearly changelog for an overview on major changes:
https://v6.docs.ctr-electronics.com/en/latest/docs/yearly-changes/yearly-changelog.html

For a list of all the changes, see the changelog:
https://api.ctr-electronics.com/changelog

## CANivore Driver Installation

> [!IMPORTANT]  
>  CANivore functionality on roboRIO 2026.1.0 requires manual installation of the CANivore driver. The CANivore **stat** LED will blink orange until this is resolved. This will be resolved in the next NI release.

1. Download the kernel driver [here](https://ctre.download/files/canivore-usb-kernel_1.16_armv7a.ipk).
2. Transfer the kernel driver (see the WPILib documentation [here](https://docs.wpilib.org/en/stable/docs/software/roborio-info/roborio-ftp.html)).
3. SSH as administrator.
4. Verify current directory contains the kernel driver with `ls`
5. Install the kernel driver with `opkg install canivore-usb-kernel_1.16_armv7a.ipk`
6. Reboot the roboRIO (CANivore stat light should now be blinking GREEN).

## Phoenix Installation
Users for all programming languages can install Phoenix by following the instructions available in our documentation:
https://v6.docs.ctr-electronics.com/en/latest/docs/installation/installation-frc.html

### Phoenix 6 Vendordep URL
- General Use: https://maven.ctr-electronics.com/release/com/ctre/phoenix6/latest/Phoenix6-frc2026-beta-latest.json
- Replay: https://maven.ctr-electronics.com/release/com/ctre/phoenix6/latest/Phoenix6-replay-frc2026-beta-latest.json

### Phoenix 5 Vendordep URL
- General Use: https://maven.ctr-electronics.com/release/com/ctre/phoenix/Phoenix5-frc2026-beta-latest.json
- Phoenix 6 Replay Compatibility
   - Please use the below vendordep when doing Phoenix 6 replay in a robot program that has Phoenix 5 devices
   - Compatibility Vendordep: https://maven.ctr-electronics.com/release/com/ctre/phoenix/Phoenix5-replay-frc2026-beta-latest.json

## API Documentation:

v6 Java: https://api.ctr-electronics.com/phoenix6/latest/java/
v6 C++: https://api.ctr-electronics.com/phoenix6/latest/cpp/
v6 Python: https://api.ctr-electronics.com/phoenix6/latest/python/

v5: Java: https://api.ctr-electronics.com/phoenix/latest/java/
v5: C++:  https://api.ctr-electronics.com/phoenix/latest/cpp/

## Phoenix Tuner X

Phoenix Tuner X is available through the app stores.

- Users on Windows should use ["Phoenix Tuner X Preview"](https://apps.microsoft.com/store/detail/9N17NS6NM06V) for the beta
- Users on macOS and iOS can join the [TestFlight](https://testflight.apple.com/join/wYhY6eQB)
Otherwise, see documentation [here](https://v6.docs.ctr-electronics.com/en/latest/docs/tuner/index.html) on how to install and use Tuner X.

## Docs and Info

Documentation for all Phoenix software is available at our landing page:
https://docs.ctr-electronics.com/
