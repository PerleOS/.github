<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/PerleOS/.github/main/profile/perleos-logo-dark-theme.svg">
    <img src="https://raw.githubusercontent.com/PerleOS/.github/main/profile/perleos-logo-light-theme.svg" alt="PerleOS" width="360">
  </picture>
</p>

PerleOS is a free Android distribution based on [LineageOS](https://lineageos.org) 24 (Android 17) for the Lenovo Tab P11 Pro **TB-J706F** (Wi-Fi). It builds its kernel from source and its vendor image from the stock firmware's proprietary files, and ships [microG](https://microg.org) instead of Google services.

PerleOS is an independent project. It is not affiliated with, endorsed by or sponsored by Lenovo, Google or the LineageOS project. Product names are used only to identify compatible hardware.

### What it adds to LineageOS

- **microG** and F-Droid, with signature spoofing limited to microG on `user` builds
- **Kernel from source**, built with the ROM, with the BPF backports that let Android 17 run on the 4.14 kernel
- **Device support**: speakers that follow the screen rotation, power-button fingerprint sensor, keyboard pack and pen
- **Its own look**: boot animation and wallpaper

### Devices

| Device | Codename | Status |
|---|---|---|
| Lenovo Tab P11 Pro TB-J706F (Wi-Fi) | `j706f` | In development, no build released |
| Lenovo Tab P11 Pro TB-J706L (LTE) | `j706l` | Planned, needs a tester who owns the device |

Other Tab P11 models use different hardware and are not supported.

### Repositories

| Repository | Content |
|---|---|
| [`local_manifests`](https://github.com/PerleOS/local_manifests) | Start here: adds PerleOS to a LineageOS 24 checkout |
| [`android_device_lenovo_pearl-common`](https://github.com/PerleOS/android_device_lenovo_pearl-common), [`android_device_lenovo_j706f`](https://github.com/PerleOS/android_device_lenovo_j706f) | Device trees |
| [`android_kernel_lenovo_sm6150`](https://github.com/PerleOS/android_kernel_lenovo_sm6150) | Kernel source |
| [`android_vendor_perleos`](https://github.com/PerleOS/android_vendor_perleos) | Product configuration and branding |
| [`android_vendor_microg`](https://github.com/PerleOS/android_vendor_microg) | microG and F-Droid prebuilts |

The other repositories are forks of LineageOS projects with small changes; [`local_manifests`](https://github.com/PerleOS/local_manifests#contents) lists each one and why it exists. The `lineage-21.0` branches (Android 14) are kept but no longer the default.

### Warning

Installing PerleOS requires an unlocked bootloader and erases the tablet. A wrong flashing step can make the device unbootable. No build is released and there is no installation guide yet; keep the stock firmware at hand.
