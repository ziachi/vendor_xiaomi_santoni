# Vendor blobs — Xiaomi Redmi 4X (santoni)

Proprietary vendor blobs for Matrixx 15 (Android 15) build.

## Info

| Detail | Value |
|--------|-------|
| Device | Xiaomi Redmi 4X (santoni) |
| Blobs | 926 files |
| Branch | `matrixx-15` |
| Path | `vendor/xiaomi/santoni` |

## Usage

This repo is automatically pulled by the device tree via `lineage.dependencies` or `local_manifests`.

```bash
git clone https://github.com/ziachi/vendor_xiaomi_santoni -b matrixx-15 vendor/xiaomi/santoni
```

## v4 Changes
- Dolby APKs, permissions, and Android.bp modules removed (no DAX hardware on santoni)
- Dolby vendor HAL `.so` files kept (other audio libs link to them, service disabled via init RC)
- All vendor blobs patchelf'd for libstdc++.so compatibility (camera, fingerprint)

## Related Repos
- [Device tree](https://github.com/ziachi/device_xiaomi_santoni/tree/matrixx-15)
- [Kernel](https://github.com/ziachi/kernel_xiaomi_msm8937/tree/matrixx-15)

---

## Thanks To
- [androidsantoni](https://github.com/androidsantoni/vendor_xiaomi_santoni) — original vendor blobs base
- [omansh-krishn](https://github.com/omansh-krishn) — thanks for keeping the source alive
- [LineageOS](https://github.com/LineageOS) — vendor extraction tools & framework
