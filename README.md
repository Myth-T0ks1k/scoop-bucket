# Mythaia — Scoop bucket

[![Tests](https://github.com/Myth-T0ks1k/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/Myth-T0ks1k/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/Myth-T0ks1k/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/Myth-T0ks1k/scoop-bucket/actions/workflows/excavator.yml)

[Scoop](https://scoop.sh) manifests for [Mythaia Pro](https://github.com/Myth-T0ks1k/Mythaia), a proxy
client for Windows: VLESS and Reality, Hysteria2, TUIC, Trojan, Shadowsocks and WireGuard, with a system
proxy or full TUN mode.

## Install

```pwsh
scoop bucket add mythaia https://github.com/Myth-T0ks1k/scoop-bucket
scoop install mythaia/mythaia-pro
```

Update with `scoop update mythaia-pro`. The manifest follows the
[releases](https://github.com/Myth-T0ks1k/Mythaia/releases) on its own: the Excavator workflow checks for
a new version every four hours and takes the hash from the release's `SHA256SUMS.txt`.

| Manifest | What it installs |
|---|---|
| [`mythaia-pro`](bucket/mythaia-pro.json) | The portable Windows x64 build, with a Start menu shortcut |

Settings and servers live in `%APPDATA%\Mythaia`, outside the Scoop folder, so they survive updates
and reinstalls.

Problems with the app itself belong in the [Mythaia repository](https://github.com/Myth-T0ks1k/Mythaia/issues);
problems with the manifest, here.
